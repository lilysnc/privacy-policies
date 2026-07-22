---
layout: default
title: 개미 은퇴 대작전 개인정보처리방침
description: 개미 은퇴 대작전의 Firebase용 Google Analytics, 플랫폼별 광고, 선택적 시장 정보 요청과 이용자 권리를 안내합니다.
permalink: /stock-game/
---

# 개미 은퇴 대작전 개인정보처리방침

> 문서 상태: 최종본 / Firebase Analytics 및 플랫폼별 광고 포함 배포본 기준<br>
> 최초 작성일: 2026년 7월 22일<br>
> 시행일: 2026년 7월 22일<br>
> 공개 개발자명: 릴리게임즈<br>
> 운영 주체: 릴리에스앤씨<br>
> 개인정보 문의: [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com)<br>
> 적용 서비스: `개미 은퇴 대작전`<br>
> Android 패키지명: `com.lilyunni.stockgame`<br>
> 개인정보처리방침 URL: https://lilysnc.github.io/privacy-policies/stock-game/

## 1. 기본 원칙과 적용 범위

`개미 은퇴 대작전`의 운영 주체인 릴리에스앤씨(공개 개발자명: 릴리게임즈, 이하 “운영자”)는 관련 법령을 준수하며 이 방침을 통해 서비스의 정보 처리와 이용자 권리를 안내합니다.

이 방침은 다음 배포 환경에 적용됩니다.

- 일반 웹
- Apps-in-Toss 미니앱
- 게임 웹 자산을 APK/AAB에 포함한 Google Play Android WebView 앱

서비스에는 회원가입, 로그인, 프로필, 채팅, 이용자 게시물, 인앱 결제, 실제 금융 거래, 클라우드 게임 저장 또는 운영자 자체 게임 기록 서버가 없습니다. 모든 프로덕션 배포판은 공유 Firebase JavaScript Web SDK의 Google Analytics를 사용합니다. 광고 SDK와 플랫폼 사업자가 자신의 서비스 제공을 위해 처리하는 정보에는 각 사업자의 방침도 적용됩니다.

## 2. 개인정보 처리 요약

| 구분 | 현재 처리 내용 |
| --- | --- |
| 앱 내 계정·로그인 | 없음 |
| 운영자 자체 서버 게임 기록 | 없음 |
| Firebase용 Google Analytics | 모든 프로덕션 배포판에서 자동 페이지·최초 방문·세션·참여 이벤트와 브라우저·기기·대략적 위치·가명 클라이언트 식별 정보를 처리할 수 있음 |
| Analytics 시작·철회 | 실행 후 즉시 초기화하며 별도 동의·철회 UI 없음 |
| 커스텀 게임 이벤트 | 게임 시작, 정답·오답, 문제 내용, 자산, 게임 종료와 광고 결과를 전송하지 않음 |
| 광고 | Android는 AdMob·UMP, Apps-in-Toss는 Toss Ads, 일반 웹은 허용된 환경의 쿠팡 파트너스 사용 |
| 위험 권한 | 위치·연락처·사진·카메라·마이크 권한 요청 안 함 |
| 로컬 저장 | 음소거 설정과 Analytics 자사 쿠키·브라우저/WebView 저장소 |
| 원격 오류 수집 | Firebase Crashlytics 등 별도 원격 오류 수집 SDK 사용 안 함 |
| 선택적 네트워크 | 경제 뉴스와 시장 지수를 위한 운영 API 요청 |

## 3. 기기 안에 저장되는 정보

음소거 설정은 브라우저 또는 WebView의 Local Storage에 저장되며 사이트·앱 데이터 삭제 또는 앱 제거 시까지 유지될 수 있습니다. 현재 문제, 자산과 체력 등 한 판의 진행 상태는 실행 중인 메모리에만 두고 페이지나 앱이 종료되면 사라집니다.

Firebase용 Google Analytics는 이용자와 세션을 구분하기 위해 자사 쿠키 `_ga`, 브라우저·WebView 저장소와 가명 클라이언트 식별자를 사용할 수 있습니다. 쿠키나 앱·사이트 데이터를 삭제하면 해당 기기의 로컬 식별자는 제거되지만 Google이 이미 처리한 집계·이벤트가 소급 삭제되는 것은 아닙니다.

## 4. 운영자가 직접 입력받지 않는 정보

운영자는 서비스 화면을 통해 이름, 생년월일, 성별, 계정 비밀번호, 이메일 주소, 전화번호, 주소, 정확한 위치, 연락처, 사진, 카메라·마이크 입력, 결제·금융·실제 거래 정보 또는 건강·생체정보를 입력받지 않습니다.

다만 Firebase용 Google Analytics, 광고 SDK, 배포 플랫폼과 호스팅 사업자는 아래 조항에 따라 IP 주소, 대략적인 위치, 브라우저·기기 정보, 서비스·광고 상호작용, 진단 정보와 가명 또는 기기 식별 정보를 자동 처리할 수 있습니다.

## 5. Firebase용 Google Analytics

일반 웹, Apps-in-Toss와 Google Play Android WebView 배포판은 Firebase JavaScript Web SDK의 Google Analytics를 앱 실행 후 즉시 초기화합니다. 별도 분석 동의 화면이나 분석 철회 설정은 제공하지 않습니다.

SDK는 자동 페이지 조회, 최초 방문, 세션 시작과 이용 시간 등 자동 이벤트를 처리할 수 있고, 페이지 URL·제목·referrer, 이벤트 시각, 브라우저·기기·운영체제·언어, IP 주소에서 추정되는 대략적 위치, 자사 쿠키·브라우저 저장소의 가명 식별 정보를 처리할 수 있습니다.

서비스는 게임 시작, 정답·오답, 문제 내용, 자산, 게임 종료 또는 광고 결과를 커스텀 Analytics 이벤트로 전송하지 않고 `setUserId`와 사용자 속성을 설정하지 않습니다. Google Signals와 광고 개인화 신호는 코드에서 비활성화합니다. 개발 모드와 자동화 브라우저에서는 초기화하지 않습니다. 실행 환경이 Firebase Analytics를 지원하지 않거나 통신이 실패해도 게임은 정상 동작합니다.

- [Google Analytics 기본 데이터 수집 안내](https://support.google.com/analytics/answer/11593727?hl=ko)
- [Firebase 개인정보 보호와 보안](https://firebase.google.com/support/privacy?hl=ko)
- [Google 개인정보처리방침](https://policies.google.com/privacy?hl=ko)

## 6. 선택적 시장 정보와 호스팅

경제 뉴스와 시장 지수를 표시하기 위해 서비스는 운영 API에 요청할 수 있습니다. 통신 과정에서 IP 주소, 사용자 에이전트와 요청 시각 등 일반 접속 정보가 Cloudflare 또는 Vercel 같은 호스팅 사업자에 의해 처리될 수 있습니다. 운영자는 이를 별도 게임 기록 데이터베이스에 복사하지 않습니다. 요청이 실패하거나 오프라인이어도 핵심 게임은 동작합니다.

- [Cloudflare 개인정보처리방침](https://www.cloudflare.com/privacypolicy/)
- [Vercel 개인정보처리방침](https://vercel.com/legal/privacy-policy)

## 7. 플랫폼별 광고와 개인정보 선택

Google Play Android 앱은 Google AdMob과 UMP를 사용해 배너·전면·리워드 광고를 제공하고 적용 지역의 광고 개인정보 선택을 관리합니다. 리워드 광고는 이용자가 보상 버튼을 선택할 때만 시작되고 SDK가 보상 완료를 알린 경우에만 혜택을 지급합니다.

Apps-in-Toss는 Toss Ads 배너·전면·리워드 광고를 사용합니다. 일반 웹은 허용된 배포 환경에서만 쿠팡 파트너스 배너를 표시합니다.

광고 SDK와 플랫폼은 광고 제공·측정, 빈도 제어, 진단, 보안과 부정 사용 방지를 위해 IP 주소, 대략적 위치, 앱·광고 상호작용, 진단 정보와 기기 또는 기타 식별자를 처리할 수 있습니다. Android UMP 개인정보 설정은 AdMob 광고 요청을 관리하며 Firebase용 Google Analytics 수집을 제어하지 않습니다.

- [Google 광고 기술에서 사용하는 정보](https://policies.google.com/technologies/ads?hl=ko)
- [Google Mobile Ads 개인정보 보호 안내](https://developers.google.com/admob/android/privacy)
- [토스 개인정보처리방침](https://toss.im/privacy)

## 8. 고객 문의 과정의 처리

이용자가 [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com)으로 문의하면 발신 이메일 주소, 문의 제목·본문과 자발적으로 첨부한 정보가 문의 확인과 회신을 위해 처리될 수 있습니다. 이용자는 문의에 불필요한 개인정보를 보내지 않아야 하며 운영자는 문의 목적에 필요하지 않은 정보를 확인하면 삭제합니다. 법령상 보존 의무가 있는 경우에는 그 기간과 범위에서 처리합니다.

## 9. 제3자 처리와 국외 처리

| 제공자 | 처리 목적 | 처리될 수 있는 정보 | 시기·방법과 보유 기준 |
| --- | --- | --- | --- |
| Google LLC — Firebase용 Google Analytics | 이용자 수·세션과 서비스 이용 현황 분석 | 자동 이벤트, 페이지·브라우저·기기·언어 정보, 대략적 위치, 가명 클라이언트 식별 정보 | 프로덕션 서비스 실행 중 HTTPS 통신; Google Analytics 속성 설정과 Google 정책에 따른 기간 |
| Google LLC — AdMob·UMP | Android 광고·동의 제공과 측정, 진단, 보안 | IP 주소, 대략적 위치, 앱·광고 상호작용, 진단 정보, 기기 또는 기타 식별자와 동의 상태 | Android 광고·동의 기능 사용 시 HTTPS 통신; Google 정책과 이용자 선택에 따른 기간 |
| 주식회사 비바리퍼블리카 — Apps-in-Toss·Toss Ads | 미니앱 실행과 광고 제공·측정·보안 | 플랫폼·기기·네트워크·광고 상호작용과 진단 관련 정보 | Apps-in-Toss 사용 시 플랫폼 통신; 토스 정책과 설정에 따른 기간 |
| Cloudflare, Inc. / Vercel Inc. | 선택적 시장 API와 웹 호스팅·보안 | IP 주소, 사용자 에이전트, 요청 URL·시각과 접속 로그 | API·웹 요청 시 HTTPS 통신; 각 사업자 정책에 따른 기간 |
| GitHub, Inc. | 개인정보처리방침 페이지 제공과 보안 | 정책 페이지 방문자의 IP 주소와 접속 로그 | 정책 페이지 접속 시 HTTPS 통신; GitHub 정책에 따른 기간 |

각 사업자의 인프라와 하위 처리자는 미국을 포함한 여러 국가에 있을 수 있습니다. 구체적인 처리 지역, 보유 기준과 권리 행사 방법은 각 사업자의 개인정보처리방침과 이용자 설정을 따릅니다.

- [Google 개인정보처리방침](https://policies.google.com/privacy?hl=ko)
- [토스 개인정보처리방침](https://toss.im/privacy)
- [Cloudflare 개인정보처리방침](https://www.cloudflare.com/privacypolicy/)
- [Vercel 개인정보처리방침](https://vercel.com/legal/privacy-policy)
- [GitHub 개인정보처리방침](https://docs.github.com/ko/site-policy/privacy-policies/github-general-privacy-statement)

## 10. 보유·삭제와 이용자 권리

운영자는 이름·이메일·계정 ID와 연결된 게임 기록을 자체 서버에 저장하지 않습니다. 이용자는 브라우저 쿠키·사이트 데이터 삭제, Android 앱 데이터 삭제 또는 앱 제거로 기기 저장 정보를 삭제할 수 있습니다. 로컬 데이터 삭제는 Google이 이미 처리한 Analytics 집계·이벤트를 소급 삭제하지 않으며, 서비스를 다시 실행하면 Analytics 수집과 새 로컬 식별자 생성이 다시 시작될 수 있습니다.

Android의 광고 설정과 앱에 표시되는 UMP 진입점으로 광고 선택을 관리할 수 있습니다. 운영자가 보유한 문의 정보의 열람, 정정, 삭제 또는 처리정지는 개인정보 문의 이메일로 요청할 수 있습니다. Google, 토스, GitHub와 호스팅 사업자가 독립적으로 처리한 정보는 각 사업자의 개인정보 도구와 창구를 이용해야 합니다.

## 11. 만 14세 미만 아동

서비스는 아동을 주 대상으로 설계하지 않았고 나이·생년월일을 직접 수집하지 않습니다. 만 14세 미만 이용자는 법정대리인과 함께 서비스 이용 및 기기·광고 개인정보 설정을 관리해야 합니다. 법정대리인의 동의 없이 아동의 개인정보가 문의에 포함된 사실을 확인하면 문의 처리에 필요한 경우를 제외하고 삭제합니다.

## 12. 안전성 확보 조치

- 분석·광고·선택적 API 통신에 HTTPS 사용
- 위치·연락처·사진·카메라·마이크 권한 요청 안 함
- 회원 비밀번호·결제 정보·실제 금융 계좌 정보 수집 안 함
- 커스텀 Analytics 게임 이벤트, 사용자 ID와 사용자 속성 전송 안 함
- Google Signals와 광고 개인화 신호 비활성화
- Analytics 실패와 게임 부팅·오프라인 동작 분리
- 운영 계정 접근 제한과 새 SDK 도입 전 데이터 흐름·스토어 고지 재검토

## 13. 문의처와 시행일

- 공개 개발자명: 릴리게임즈
- 운영 주체: 릴리에스앤씨
- 개인정보 문의: [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com)

이 방침은 2026년 7월 22일부터 시행합니다.

## 14. 방침 변경과 변경 이력

기능, 분석, 광고 SDK, 플랫폼 또는 법적 요구사항이 변경되면 시행일과 함께 이 방침을 갱신합니다.

- 2026년 7월 22일: 최초 개인정보처리방침 작성
- 2026년 7월 22일: 세 프로덕션 배포판의 Firebase용 Google Analytics 즉시 자동 수집, 플랫폼별 광고와 선택적 시장 정보 처리 반영
