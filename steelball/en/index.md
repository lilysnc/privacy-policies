---
layout: default
lang: en
title: Steelball Go Privacy Policy
description: How Steelball Go handles advertising and consent, analytics, Apps in Toss promotions and leaderboards, on-device storage, and your privacy rights.
brand: Lilygames Privacy Policy
repo_label: Policy repository
permalink: /steelball/en/
---

# Steelball Go Privacy Policy

> Other languages: [한국어](../)

> Document status: Revised / covers rewarded ads, Apps in Toss promotions and leaderboards, written for global distribution<br>
> First published: 3 August 2026<br>
> Last revised: 12 August 2026<br>
> Effective date: 12 August 2026<br>
> Publisher name: Lilygames<br>
> Legal entity: LilySnC<br>
> Privacy contact: [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com)<br>
> Service: `Steelball Go` (Korean title `스틸볼런`)<br>
> Android package name: `com.lilysnc.steelball`<br>
> Apps in Toss app name: `steelball`<br>
> Privacy policy URL: https://lilysnc.github.io/privacy-policies/steelball/en/

## 1. Scope and per-build data flows

LilySnC (publisher name: Lilygames; "we", "us") operates `Steelball Go`. We respect your privacy and comply with applicable law, including the Personal Information Protection Act (Republic of Korea), the GDPR and UK GDPR (European Economic Area, United Kingdom and Switzerland), and US state privacy laws.

This policy covers the three builds below. **Data flows differ by build**, so we state them first.

| Build | Advertising | Analytics events sent | Promotions and leaderboard | Storage location |
| --- | --- | --- | --- | --- |
| Google Play Android app | Google Mobile Ads (AdMob) banner, interstitial and rewarded | Sent to Firebase Analytics | None | On-device native storage |
| Apps in Toss game mini app | Banner, interstitial and rewarded surfaces provided by Toss | **Not sent** | Toss promotion payouts, Toss Game Center leaderboard | Toss app storage |
| Browser build (development and QA) | None | **Not sent** | None | Browser `localStorage` |

- The Apps in Toss build does not include the AdMob SDK, and the Google Play build does not include the Apps in Toss SDK.
- The Apps in Toss and browser builds have no path for sending analytics events at all. Events the game produces never leave the device; they are discarded.
- The service has **no sign-up, no login, no chat, no user-generated posts, no cloud save and no server of ours.** We do not operate an API server, an account system or a database.
- In-app purchases are not offered at present. If we add them, we will update this policy before releasing the build that contains them.

Where platform or SDK providers such as Google, Toss and GitHub process information independently to operate their own services, their privacy policies apply in addition to this one.

## 2. Summary of information we process

| Category | What happens |
| --- | --- |
| In-app account or login | None |
| Information sent to a server of ours | None |
| User identifier created by us | None. We do not create or store any value that persistently identifies a device or a person |
| Session identifier | A random value (`session_id`) generated fresh on every app launch. It is not stored and disappears when the app closes |
| Advertising | Banner, interstitial and rewarded ads (section 4) |
| Automated processing for advertising | Advertising identifier, approximate location inferred from IP address, device and app information, ad request, impression and interaction data, consent signals |
| Advertising consent and choices | Where consent is required, it is collected before any ad request, and you can reopen and change it at any time from **`Settings > Ad settings`** inside the game (section 5) |
| Analytics | Only the **Google Play build** sends gameplay events to Firebase Analytics (section 6) |
| Apps in Toss promotions | When payout conditions are met we pass Toss only a promotion code and an amount. Toss identifies the recipient and performs the payout (section 7) |
| Leaderboard | The Apps in Toss build submits a single integer — your personal best — to the Toss Game Center. We do not send a nickname or profile (section 7) |
| Crash reporting SDK | None (no Crashlytics or equivalent) |
| Sensitive permissions | We do not request location, contacts, photos, camera, microphone, storage or notification permissions |
| On-device storage | Game progress, promotion payout ledger, audio settings, language setting (section 8) |
| Information you send us directly | Your sending email address, the content of your enquiry, and anything you choose to attach |
| Sale of personal information | We do not sell your information to third parties for money or other valuable consideration |
| Sensitive data or child-directed processing | None |

Non-personalised or limited ads still process some IP address, device or diagnostic information for ad delivery, frequency capping, security and fraud prevention. "Non-personalised ads" therefore does not mean that all data processing stops.

## 3. Purposes and legal bases

The following bases apply to users in regions covered by the GDPR and UK GDPR. In the Republic of Korea, the corresponding bases under the Personal Information Protection Act are consent, performance of a contract, or legitimate interests.

| Processing activity | Purpose | GDPR legal basis |
| --- | --- | --- |
| Running the game and saving progress | Providing the service | Performance of a contract (Art. 6(1)(b)) |
| Personalised advertising and use of the advertising identifier | Funding a free service | **Consent** (Art. 6(1)(a)). Without consent we request only non-personalised ads |
| Ad delivery, frequency capping and fraud prevention | Making the advertising function work, and security | Legitimate interests (Art. 6(1)(f)) or consent |
| Gameplay analytics | Detecting errors, improving difficulty and features | Legitimate interests (Art. 6(1)(f)) |
| Handling enquiries | Responding to your requests and complaints | Performance of a contract or legitimate interests |
| Legal compliance | Age rating, accounting, dispute handling | Legal obligation (Art. 6(1)(c)) |

## 4. Advertising

### 4.1 Banner

The banner is a **single surface that stays at the bottom of every screen**. The game reserves exactly the height the SDK reports, so the banner never covers controls or gameplay elements. If no ad is filled or the ad cannot render, the reserved space is reclaimed immediately.

### 4.2 Interstitial ads

An interstitial is only a candidate on the transition after you press `Roll Again` on the result screen. It additionally requires a minimum number of runs since the last impression, a minimum amount of accumulated active play, and a full-screen overlay cooldown. It is never shown during the first-run practice course or your first two runs. If the ad fails to load, the next run starts immediately without an ad.

### 4.3 Rewarded ads

Rewarded ads only play **when you start them yourself**; they are never shown automatically. There are three places where they are offered:

- Continuing a run once, after you have travelled at least a set distance in that run
- Refilling one heart (a recorded-run ticket) when you have none left
- Continuing from a checkpoint after failing a course

A reward is granted only when the ad provider confirms that you finished watching. If you dismiss the ad or it fails to load, you return to the previous screen without a reward.

### 4.4 Ad providers

| Build | Ad provider |
| --- | --- |
| Google Play | Google Mobile Ads (AdMob) |
| Apps in Toss | Ad surfaces provided by Toss (Toss advertising and AdMob mediated by Toss) |
| Browser | None |

We never give in-game gold, score multipliers or ranking advantages in exchange for watching an ad.

## 5. Advertising consent and your choices

### 5.1 European Economic Area, United Kingdom and Switzerland

The Google Play build uses the Google User Messaging Platform (UMP) to collect consent **before any ad request**. If you do not consent, we do not request personalised ads; if the consent flow does not permit ad requests, we do not request ads at all.

You can reopen the consent screen and change or withdraw your choice at any time from **`Settings > Ad settings`** inside the game. This entry point is shown only in regions where consent management is required.

### 5.2 United States

Where state law requires it, the Google Play build offers an opt-out screen for the sale or sharing of personal information. We do not sell your information, and sharing for advertising purposes can be limited through that choice.

### 5.3 Device settings available everywhere

- Android Settings → Privacy → Ads: **Delete advertising ID** or **Reset advertising ID**
- Google Account → Data & privacy → Ad settings

### 5.4 Apps in Toss build

For the Apps in Toss mini app, advertising consent and ad personalisation settings are **owned and managed by Toss**. We do not display a separate consent screen there; those choices follow the Toss app settings and the [Toss Privacy Policy](https://toss.im/privacy).

## 6. Analytics (Google Play build only)

The Firebase Analytics web SDK runs **only in the Google Play build**. The Apps in Toss and browser builds have no path for sending events.

The events we send describe game progress and feature use. Representative items:

| Event type | Example values sent |
| --- | --- |
| App open | Whether the tutorial was completed |
| Run or course end | Score, distance travelled (m), elapsed time (s), failure reason, whether a continue was used, stars and gold awarded |
| Advertising flow | Surface type (banner, interstitial, rewarded), request/impression/failure/close phase, failure reason code |
| Mission and tutorial progress | Mission identifier, step number, gold awarded |
| Settings and diagnostics | Opening and closing the privacy options screen, toggling developer diagnostic mode |

Every event carries an app identifier, app version, session identifier and build mode. The session identifier is a random value created on each app launch and is not stored.

We do not put names, email addresses, phone numbers, precise location, advertising identifiers or promotion codes into analytics events. Event names and values are normalised for format, length and count before sending, and if any analytics configuration value is missing the entire analytics function is disabled.

Information that the Firebase and Google Analytics SDKs process additionally in order to provide their service — an app instance identifier, approximate location inferred from IP address, device and app information, and automatically collected events — is handled independently by Google. See [Firebase privacy and security](https://firebase.google.com/support/privacy).

**Notice about analytics and advertising consent.** In the current build, the analytics SDK is initialised independently of the advertising consent flow. We will apply analytics consent integration (Google consent mode) and release it in the build that contains it, updating this section at that time. Until then, if you are in the European Economic Area, the United Kingdom or Switzerland and do not want analytics, contact us using section 11 and we will stop the processing.

## 7. Processing in the Apps in Toss mini app

### 7.1 Promotion payouts

When defined conditions are met — cumulative confirmed interstitial impressions, a first run completed with a specific ball, a once-per-day distance milestone, a once-per-day personal-record improvement, and completing a course — the Apps in Toss build passes Toss **only a promotion code and an amount**. Toss identifies the recipient and performs the payout. We do not receive your Toss account details or any personal information contained in the payout result.

To prevent duplicate payouts, the payout history is stored **only on your device** (section 8). Date-keyed entries are cleared after seven days.

### 7.2 Game Center leaderboard

For runs whose result is final, the Apps in Toss build submits **a single integer, your personal best**, to the Toss Game Center. We do not send a nickname, profile image or device information; ranking display and account linkage are handled by Toss. Assisted runs (for example diagnostic mode) are not submitted. We do not operate a ranking server of our own.

## 8. Information stored on your device

We store the values below **only in device or platform local storage** and never copy them to a server of ours.

| Stored item | Contents | Purpose |
| --- | --- | --- |
| Game progress | Best distance, current and lifetime gold, unlocked and equipped cosmetics, heart count and refill reference time, tutorial completion, free-roll count, today's mission progress, values used to compute interstitial pacing, course stars and today's course play count | Restoring progress and keeping ad pacing |
| Promotion payout ledger | Payout state per milestone, cumulative interstitial values | Preventing duplicate payouts |
| Audio settings | Whether music and sound effects are on | Restoring your settings |
| Language setting | Selected language (`ko` / `en`) | Restoring your settings |

| Build | Physical storage location |
| --- | --- |
| Google Play Android app | App-private native storage (`Preferences`) |
| Apps in Toss | Mini app storage provided by the Toss app |
| Browser | Browser `localStorage` |

The stored values contain **no** name, email address, phone number, postal address, precise location, contacts or device identifier. The only time values stored are the heart refill reference time, mission completion times, and integers used to separate calendar days.

On devices where the operating system's app data backup is enabled, these values may be included in your Google account backup for the Android app. That backup is managed by Google under your account.

## 9. Third-party services, processors and international transfers

| Provider | Purpose | Information that may be processed | Applicable build |
| --- | --- | --- | --- |
| Google Mobile Ads (AdMob), Google User Messaging Platform | Delivering banner, interstitial and rewarded ads, collecting consent, measuring performance, preventing abuse | Advertising identifier, IP address, device and app information, ad request, impression and interaction data, consent signals | Google Play |
| Firebase Analytics (Google) | Analysing gameplay flow and feature quality | The events and common fields in section 6, plus device and app information Google processes to provide the service | Google Play |
| Viva Republica (Toss) | Running the mini app, providing ad surfaces, promotion payouts, Game Center leaderboard, mini app storage | Information Toss processes to operate its own services, plus the promotion code and amount and the leaderboard score we pass | Apps in Toss |
| GitHub (Microsoft) | Hosting this privacy policy page | Visitor IP address, access logs | Policy page |
| Google (email) | Receiving enquiry email | Your sending email address and the content of your enquiry | Enquiries |

Information processed by Google and GitHub may be processed on **their global infrastructure, including in the United States**. Transfers from the European Economic Area and the United Kingdom to third countries rely on the EU Standard Contractual Clauses adopted by each provider together with supplementary safeguards. Information processed by Toss is processed in the Republic of Korea.

- [Google Privacy Policy](https://policies.google.com/privacy)
- [How Google uses information from sites or apps that use our services](https://policies.google.com/technologies/partner-sites)
- [Firebase privacy and security](https://firebase.google.com/support/privacy)
- [Toss Privacy Policy](https://toss.im/privacy)
- [GitHub Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement)

## 10. Retention and deletion

We store no per-user information on any server of ours, so deletion concerns the values stored on your device and information held by third-party services.

| Subject | Retention | How to delete |
| --- | --- | --- |
| Game data stored on your device | Until you clear app data or uninstall the app | Google Play: clear `Steelball Go` storage and app data in Android Settings, or uninstall the app / Apps in Toss: remove the mini app in the Toss app / Browser: clear the site's stored data |
| Enquiry email (sender address, subject and body, attached information) | 30 days after the enquiry is resolved | Deleted after the correspondence ends. Where law requires longer retention, we keep it only to the extent and for the period that law requires |
| Information held by advertising and analytics providers | According to each provider's policy | The device settings in section 5, your Google Account data and privacy settings, or a request under section 11 |

## 11. Your rights and how to exercise them

You may exercise the rights below. If the GDPR or UK GDPR applies to you, these include the rights of access, rectification, erasure ("right to be forgotten"), restriction of processing, data portability, objection, rights regarding automated decision-making, withdrawal of consent, and lodging a complaint with a supervisory authority. If a US state privacy law applies to you, these include the rights to know, delete, correct, opt out of sale and sharing, and not to be discriminated against for exercising them.

**How to exercise**

- Game data stored on your device can be deleted directly using the methods in section 10.
- Advertising consent can be changed or withdrawn at any time from `Settings > Ad settings` inside the game (in applicable regions).
- For anything else, write to [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com). Where verification is needed we check the minimum necessary information, and we respond within 30 days of receipt (one month under the GDPR, extendable by two further months with notice of the reason).
- Because we operate no accounts, an email address alone does not let us locate a particular user's on-device data. In that case deletion can only be completed with the device deletion methods above.

**Supervisory authorities and dispute resolution**

- Republic of Korea: Privacy Infringement Report Centre https://privacy.kisa.or.kr (118) · Personal Information Dispute Mediation Committee https://www.kopico.go.kr (1833-6972) · National Police Agency Cybercrime Reporting System https://ecrm.police.go.kr (182)
- European Economic Area, United Kingdom and Switzerland: you may lodge a complaint with the data protection authority in your country of residence. See https://edpb.europa.eu/about-edpb/about-edpb/members_en for European authorities and https://ico.org.uk for the United Kingdom.

## 12. Children's privacy

The app is intended for users aged 13 and over. It is not designed for or directed primarily at children, it never asks children to enter personal information, and we do not process information for the purpose of child-directed personalised advertising.

- Republic of Korea: a user under the age of 14 who needs to contact us must do so through a legal guardian.
- European Economic Area and United Kingdom: if you are below the digital consent age set by your country (13 to 16), a legal guardian's consent is required.
- United States: we do not knowingly collect personal information from children under 13. If we learn that we have, we delete it without delay.

## 13. Security measures

- The app has no personal information input screen and we operate no account system.
- Game data is stored only in device or platform storage and is never copied to a server of ours.
- We request no sensitive permissions. The Android app declares only two: internet access and access to the advertising identifier.
- Cleartext HTTP is not permitted; all external communication uses HTTPS through the SDKs.
- Advertising identifiers (ad application ID, ad unit IDs) and promotion codes are injected only through build configuration and are never written to analytics events or logs.
- A pre-submission verification step checks that test advertising identifiers and diagnostic flags are absent from release artefacts.
- Before adopting a new SDK or network feature, we review permissions, the consent flow and the resulting data flows again.

## 14. Update rules and notice of changes

If we add or change advertising, analytics, login, payments, cloud save, crash reporting, communication with an external server, a new distribution platform (for example the Apple App Store), or any other feature that processes personal information, we update this policy together with the Google Play Data safety declaration and the Apps in Toss console information **before releasing the build that contains it**.

When we change this policy we announce the change and its effective date on this page or through the store listing. As a rule we give 30 days' notice before a change that materially affects your rights, and 7 days' notice for other changes. **Corrections** made to describe features that are already live accurately take effect immediately.

## 15. Contact and effective date

- Publisher name: Lilygames
- Legal entity: LilySnC
- Privacy contact: [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com)

This policy takes effect on **12 August 2026**.

## Change history

- 12 August 2026: Fully revised for global distribution. Added the three rewarded ad placements and the always-present banner surface, Apps in Toss promotion payouts and the Game Center leaderboard, and the differences in data flow between builds. Added GDPR and UK GDPR legal bases and data subject rights, US state privacy choices, the basis for international transfers, and supervisory authority information. Documented the in-game `Settings > Ad settings` consent withdrawal entry point and the current relationship between analytics and advertising consent, and updated the on-device storage list to the current schema. Published this English version alongside the Korean one.
- 3 August 2026: Clarified, on the basis of distribution in the Republic of Korea only, that the GDPR consent form (UMP) was not used, and described ad personalisation controls in terms of device settings.
- 3 August 2026: Reflected the Google Play build's AdMob banner and interstitial ads, Firebase Analytics events and common fields, advertising identifier processing, processing outside Korea, and the controls available to users.
- 3 August 2026: First written and published on GitHub Pages for a minimal build with no advertising, analytics or network communication.
