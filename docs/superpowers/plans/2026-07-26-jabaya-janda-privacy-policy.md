# 잡아야 잔다 개인정보처리방침 Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** `잡아야 잔다`의 Android·iOS·웹 실제 데이터 흐름을 반영한 개인정보처리방침을 기존 GitHub Pages 저장소에 게시하고 공개 URL을 검증한다.

**Architecture:** 기존 Jekyll 정책 저장소의 게임별 디렉터리 패턴을 재사용한다. `jabaya-janda/index.md`가 정책 원문과 고정 permalink를 소유하고, 루트 `index.md`와 `README.md`는 탐색 링크만 제공한다. 원본 앱 저장소의 Play Console 안내 URL도 새 정책 주소로 맞춘다.

**Tech Stack:** Jekyll, GitHub Pages, Markdown, Git, HTTP

## Global Constraints

- 정책 적용 범위는 Google Play Android 앱, App Store iOS 앱, `https://jabaya-janda.pages.dev/` 웹 버전이다.
- 서비스명은 `잡아야 잔다`, 앱 식별자는 Android/iOS 모두 `com.lilysnc.jabaya`이다.
- 공개 개발자명은 `릴리게임즈`, 운영 주체는 `릴리에스앤씨`, 개인정보 문의는 `lilygames@lilysnc.com`이다.
- 공개 정책 URL은 `https://lilysnc.github.io/privacy-policies/jabaya-janda/`이다.
- Android/iOS 네이티브 앱만 Google Mobile Ads SDK의 배너·전면 광고를 사용하며 보상형 광고는 없다.
- Android는 `AD_ID` 권한을 사용하고, iOS는 ATT 추적 권한을 요청할 수 있다. 권한 거부는 핵심 게임 이용을 막지 않는다.
- 웹 버전에는 AdMob, Firebase Analytics, Crashlytics 또는 다른 분석 SDK가 없다.
- 앱에는 계정, 로그인, 결제, 채팅, 운영자 게임 서버, 영구 게임 진행 저장이 없다.
- Google Mobile Ads SDK가 자동 처리할 수 있는 IP 주소 기반 대략적 위치, 앱·광고 상호작용, 진단 정보, 기기·계정 식별자를 고지한다.
- 정책 문서는 법률 자문이 아니며 Google Play 데이터 보안 양식은 실제 배포 SDK 기준으로 별도 유지한다.

---

### Task 1: 다중 플랫폼 개인정보처리방침 작성

**Files:**
- Create: `jabaya-janda/index.md`

**Interfaces:**
- Consumes: `_layouts/default.html`, `_config.yml`의 `baseurl: /privacy-policies`
- Produces: permalink `/jabaya-janda/`와 공개 URL `https://lilysnc.github.io/privacy-policies/jabaya-janda/`

- [x] **Step 1: 정책 문서 뼈대와 운영 정보 작성**

Front matter는 다음 값을 사용한다.

```yaml
---
layout: default
title: 잡아야 잔다 개인정보처리방침
description: 잡아야 잔다의 플랫폼별 광고, 추적 권한, 호스팅 정보와 이용자 권리를 안내합니다.
permalink: /jabaya-janda/
---
```

문서 상단에 최초 작성일·시행일 `2026년 7월 26일`, 공개 개발자명, 운영 주체, 문의 이메일, 서비스명, Android/iOS 식별자, 웹 서비스 URL, 정책 URL을 명시한다.

- [x] **Step 2: 실제 데이터 처리와 플랫폼 차이 작성**

다음 항목을 각각 독립된 절로 작성한다.

1. 적용 범위와 기본 원칙
2. 개인정보 처리 요약 표
3. 게임 상태와 기기 저장: 게임 진행·음향 설정은 실행 중 메모리만 사용하며 종료 시 유지하지 않음
4. 앱이 직접 수집하지 않는 정보: 계정·연락처·위치·미디어·금융·민감정보 없음
5. Android/iOS 광고: 배너·전면 광고, 보상형 광고 없음, Android AD_ID, iOS ATT, 거부 시 핵심 기능 유지
6. Google Mobile Ads 처리 가능 정보: IP 기반 대략적 위치, 사용자 제품 상호작용, 진단, 기기·계정 식별자
7. 웹 버전: 광고·분석 SDK 없음, Cloudflare 정적 호스팅 로그 가능성
8. 제3자·국외 처리: Google, Cloudflare, GitHub Pages, Google 메일, Google Play, Apple App Store
9. 문의 정보: 발신 이메일·본문·자발적 첨부를 문의 완료 후 30일 보유
10. 보유·삭제: 앱 삭제/데이터 삭제, 사이트 데이터 삭제, 플랫폼·SDK 정책에 따른 보유
11. 만 13세 이상 대상과 만 14세 미만 법정대리인 안내
12. 이용자 권리와 Android 광고 ID/iOS 추적 설정 경로
13. 안전성 조치, 변경 절차, 문의처, 변경 이력

- [x] **Step 3: 정책 자체 정합성 검사**

Run from `C:/PROJECTS/lilyunni/privacy-policies`:

```powershell
$policy = Get-Content -Raw -Encoding UTF8 jabaya-janda/index.md
@(
  'permalink: /jabaya-janda/',
  'com.lilysnc.jabaya',
  'lilygames@lilysnc.com',
  'Google Mobile Ads',
  'AD_ID',
  'ATT',
  'Cloudflare',
  'GitHub Pages',
  '만 13세 이상',
  '2026년 7월 26일'
) | ForEach-Object { if (-not $policy.Contains($_)) { throw "Missing policy fact: $_" } }
```

Expected: exit code 0 and no output.

### Task 2: 정책 탐색 링크와 앱 안내 정합화

**Files:**
- Modify: `index.md`
- Modify: `README.md`
- Modify: `C:/PROJECTS/lilyunni/jabaya-janda-src/README.md`
- Modify: `C:/PROJECTS/lilyunni/jabaya-janda-src/docs/superpowers/plans/2026-07-26-android-google-play-aab.md`
- Modify: `C:/PROJECTS/lilyunni/jabaya-janda-src/docs/superpowers/specs/2026-07-26-android-google-play-aab-design.md`

**Interfaces:**
- Consumes: Task 1의 `/jabaya-janda/` permalink
- Produces: 정책 허브 카드, 저장소 목록 항목, Play Console 등록용 새 URL

- [x] **Step 1: 정책 허브에 게임 카드 추가**

`index.md`의 `<ul class="policy-list">` 안에 다음 카드를 추가한다.

```html
  <li>
    <a class="policy-card" href="{{ '/jabaya-janda/' | relative_url }}">
      <strong>잡아야 잔다</strong>
      <span>Android/iOS 앱 ID: com.lilysnc.jabaya · 시행일: 2026년 7월 26일</span>
    </a>
  </li>
```

- [x] **Step 2: 정책 저장소 README에 공개 링크 추가**

게임 목록에 다음 줄을 추가한다.

```markdown
- 잡아야 잔다: https://lilysnc.github.io/privacy-policies/jabaya-janda/
```

- [x] **Step 3: 원본 앱 등록 문서의 Play Console URL 교체**

`C:/PROJECTS/lilyunni/jabaya-janda-src/README.md`, Android Google Play 구현 계획, 승인 설계 문서의 기존 `https://jabaya-janda.pages.dev/privacy.html`을 `https://lilysnc.github.io/privacy-policies/jabaya-janda/`로 교체한다.

- [x] **Step 4: 내부 링크와 단일 정식 URL 검사**

Run:

```powershell
$hub = Get-Content -Raw -Encoding UTF8 index.md
$repoReadme = Get-Content -Raw -Encoding UTF8 README.md
$appRoot = 'C:/PROJECTS/lilyunni/jabaya-janda-src'
$appReadme = Get-Content -Raw -Encoding UTF8 "$appRoot/README.md"
$appPlan = Get-Content -Raw -Encoding UTF8 "$appRoot/docs/superpowers/plans/2026-07-26-android-google-play-aab.md"
$appSpec = Get-Content -Raw -Encoding UTF8 "$appRoot/docs/superpowers/specs/2026-07-26-android-google-play-aab-design.md"
if (-not $hub.Contains("{{ '/jabaya-janda/' | relative_url }}")) { throw 'Hub link missing' }
if (-not $repoReadme.Contains('https://lilysnc.github.io/privacy-policies/jabaya-janda/')) { throw 'Repository link missing' }
@($appReadme, $appPlan, $appSpec) | ForEach-Object {
  if (-not $_.Contains('https://lilysnc.github.io/privacy-policies/jabaya-janda/')) { throw 'App registration link missing' }
  if ($_.Contains('https://jabaya-janda.pages.dev/privacy.html')) { throw 'Stale app registration link remains' }
}
```

Expected: exit code 0 and no output.

### Task 3: 커밋·게시·공개 페이지 검증

**Files:**
- Commit in: `C:/PROJECTS/lilyunni/privacy-policies`
- Commit in: `C:/PROJECTS/lilyunni/jabaya-janda-src`

**Interfaces:**
- Consumes: Task 1 policy and Task 2 links
- Produces: 정책 저장소 `origin/main` 커밋, 앱 저장소 로컬 문서 커밋, 공개 HTTPS 정책 페이지

- [x] **Step 1: 두 저장소의 변경 범위 확인**

Run `git status --short` in each repository. Expected privacy repository changes: `README.md`, `index.md`, `jabaya-janda/index.md`, this plan file. Expected app repository changes: `README.md`, the Android Google Play implementation plan, and its approved design document.

- [x] **Step 2: 앱 안내 URL 변경을 로컬 커밋**

```powershell
git add README.md docs/superpowers/plans/2026-07-26-android-google-play-aab.md docs/superpowers/specs/2026-07-26-android-google-play-aab-design.md
git commit -m "docs: point Play listing to privacy policy"
```

Expected: 원격이 구성되지 않은 앱 저장소에 로컬 문서 커밋 `a65bbef` 생성.

- [ ] **Step 3: 정책 저장소 변경 커밋·푸시**

```powershell
git add README.md index.md jabaya-janda/index.md docs/superpowers/plans/2026-07-26-jabaya-janda-privacy-policy.md
git commit -m "docs: publish jabaya janda privacy policy"
git push origin main
```

Expected: one policy commit pushed to `origin/main`.

- [ ] **Step 4: GitHub Pages 배포 완료 대기와 HTTP 확인**

정책 URL을 캐시 우회 쿼리와 함께 요청해 HTTP 200이 될 때까지 GitHub Pages 배포를 확인한다.

```powershell
$url = 'https://lilysnc.github.io/privacy-policies/jabaya-janda/?v=' + [DateTimeOffset]::UtcNow.ToUnixTimeSeconds()
$response = Invoke-WebRequest -UseBasicParsing $url
if ($response.StatusCode -ne 200) { throw "HTTP $($response.StatusCode)" }
if (-not $response.Content.Contains('잡아야 잔다 개인정보처리방침')) { throw 'Rendered title missing' }
if (-not $response.Content.Contains('com.lilysnc.jabaya')) { throw 'Rendered app ID missing' }
```

Expected: exit code 0.

- [ ] **Step 5: 브라우저 렌더링 확인**

공개 URL을 브라우저에서 열고 제목, 적용 범위, 모바일 폭 레이아웃, 외부 링크가 정상 렌더링되는지 확인한다.

- [ ] **Step 6: 최종 원격 정합성 확인**

각 저장소에서 `git status --short --branch`를 실행한다. Expected: 정책 저장소는 `main...origin/main`, 원격이 없는 앱 저장소는 `main`이며 두 저장소 모두 추적 변경이 없다.
