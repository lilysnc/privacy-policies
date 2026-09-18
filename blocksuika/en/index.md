---
layout: default
title: BlockSuika Privacy Policy
description: How BlockSuika stores data on your device, the current status of ads and analytics, third-party processing, and your rights.
permalink: /blocksuika/en/
---

# BlockSuika Privacy Policy

> Other languages: [한국어](../)

> Document status: First edition / based on the web build, which has no ads, no analytics and no server communication<br>
> First published: September 18, 2026<br>
> Last revised: September 18, 2026<br>
> Effective date: September 18, 2026<br>
> Publisher name: LilyGames<br>
> Operating entity: Lily S&C<br>
> Privacy contact: [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com)<br>
> Covered service: `BlockSuika` / Korean title `블록 스이카`<br>
> Web build address: https://blocksuika.pages.dev<br>
> Privacy policy URL: https://lilysnc.github.io/privacy-policies/blocksuika/en/

## 1. Scope and Data Flow per Build

Lily S&C (publisher name: LilyGames, the “Operator”), the operating entity of `BlockSuika`, takes your privacy seriously and complies with applicable laws including the Personal Information Protection Act (Republic of Korea), the GDPR and UK GDPR (EEA, United Kingdom, Switzerland), and U.S. state privacy laws.

This policy applies to the builds published today. Because **data flows can differ per build**, they are stated first.

| Build | Status | Ads | Analytics events sent | Storage location |
| --- | --- | --- | --- | --- |
| Web (browser) | **Published** | None | **Not sent** | Browser `localStorage` |
| Google Play Android app | Not released | Not included | Not connected | This policy is updated before release |
| Apple App Store app | Not released | Not included | Not connected | This policy is updated before release |
| Apps in Toss mini app | Not released | Not included | Not connected | This policy is updated before release |

- The only build you can play today is the **web build**, and it contains **no advertising SDK and no analytics transmission path.**
- The service has **no sign-up, no login, no chat, no user-generated posts, no cloud save, no in-app purchases, no push notifications and no Operator server.** The Operator runs no API server, account system or database.
- Image and sound assets ship inside the build; the game does not call an external content server while running.
- Information that hosting providers such as Cloudflare and GitHub process independently to run their own services is also governed by their own privacy policies.

## 2. Summary of Processing

| Item | What happens |
| --- | --- |
| In-app account or login | None |
| Data sent to an Operator server | None |
| Identifiers created by the Operator | None. No value that persistently identifies a device or user is created or stored |
| Advertising | **Not present in the published build** (Section 4) |
| Advertising identifier | Not read |
| Analytics | **Not transmitted** (Section 6) |
| Remote crash reporting SDK | Not used |
| In-app purchases or promotional payouts | None |
| Leaderboard or ranking server | None. Records stay on the device |
| Sensitive permissions | Location, contacts, photos, camera, microphone, storage and notification permissions are not requested |
| On-device storage | Game progress, in-game item and gold coin balances, daily reward record, volume settings, language setting (Section 7) |
| Access logs | When you open the web build, the hosting provider (Cloudflare) may process its own access logs (Section 8) |
| Messages you send us | Sender email address, message content and anything you attach voluntarily |
| Sale of personal information | Never. Your information is not sold to third parties for consideration |
| Sensitive data or child-directed processing | None |

The in-game “gold coins” are an **in-game currency** earned only by playing; there is no payment or cash-out feature.

## 3. Purposes and Legal Bases

For users in regions where the GDPR or UK GDPR applies, the bases below apply. In the Republic of Korea, consent or performance of a contract and legitimate interests under the Personal Information Protection Act are the corresponding bases.

| Processing activity | Purpose | GDPR legal basis |
| --- | --- | --- |
| Running the game and saving progress (on device) | Providing the service | Performance of a contract (Art. 6(1)(b)) |
| Delivering the web build and its access logs (hosting) | Service delivery, security and abuse prevention | Legitimate interests (Art. 6(1)(f)) |
| Serving this policy page (GitHub Pages) | Providing a legally required notice | Legal obligation (Art. 6(1)(c)) or legitimate interests |
| Handling enquiries | Responding to requests and complaints | Performance of a contract or legitimate interests |
| Legal compliance | Age rating, accounting, dispute handling | Legal obligation (Art. 6(1)(c)) |

## 4. Advertising

The published web build contains **no advertising.** No ad network SDK is included, no advertising identifier is read, and no ad-related external communication takes place.

The game does contain “watch an ad for a reward” style UI. In the current build that button is implemented as an **internal verification stub that grants the reward immediately without playing any external ad**, and it performs no network communication.

If real advertising is introduced, the ad providers, the data processed and the consent flow (where required) will be added to this policy **before** the build containing that feature is released (Section 13).

## 5. Your Choices and Device Settings

- **Volume and language**: In the in-game `Settings` you can change music and sound volume and the language (English or Korean); the choice is stored only on your device.
- **Deleting game data**: Clearing this site’s stored data in your browser removes everything the game saved (Section 9).
- **Ad personalisation**: The current build has no ads, so there is no related choice to make. If advertising is introduced, the consent or opt-out mechanisms required in your region will be provided with it.

## 6. Analytics

The Operator currently **sends no usage analytics events off the device.** The game contains an interface for recording events, but the implementation shipped in the published build does nothing and is not connected to any analytics service.

If an analytics service such as Firebase Analytics is connected, the event types, common fields and consent handling will be written into this policy before the build containing that feature is released.

## 7. Information Stored on Your Device

The Operator stores the values below **only in device or browser local storage** and never copies them to an Operator server.

| Stored item | Contents | Purpose |
| --- | --- | --- |
| Game progress | Best score, total games played, highest tier reached | Restoring progress and showing records |
| In-game currency and items | Gold coin balance, remaining items (hammer, bomb, gem drop, shuffle) | Restoring your holdings |
| Daily reward record | Last claim day (local day number), cycle day | Granting once per day and computing the streak |
| Settings | Music and sound volume, selected language (`ko`/`en`) | Restoring settings |

| Build | Physical storage location |
| --- | --- |
| Web (browser) | A single browser `localStorage` key (`blocksuika.save.v1`) |
| Google Play / App Store app (not released) | App-private native storage at release |
| Apps in Toss mini app (not released) | Mini app storage provided by the Toss app at release |

The stored values contain **no** name, email address, phone number, postal address, precise location, contacts, advertising identifier or device identifier. The only time information stored is a **day-level integer** used for the daily reward.

## 8. Third Parties, Processors and International Transfers

| Provider | Purpose | Information that may be processed | Applies to |
| --- | --- | --- | --- |
| Cloudflare | Serving the static files of the web build (Cloudflare Pages), security and abuse prevention | Access logs such as IP address, request time and URL, browser and device information | Web build |
| GitHub (Microsoft) | Serving this privacy policy page (GitHub Pages) | Visitor IP address, access logs | Policy page |
| Google (email) | Receiving enquiry emails | Sender email address and message content | Enquiries |

Information processed by Cloudflare, GitHub and Google may be processed on **their global infrastructure, including the United States.** Transfers from the EEA or the United Kingdom to third countries rely on the EU Standard Contractual Clauses and the additional safeguards adopted by each provider.

- [Cloudflare Privacy Policy](https://www.cloudflare.com/privacypolicy/)
- [GitHub Privacy Statement](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement)
- [Google Privacy Policy](https://policies.google.com/privacy)

## 9. Retention and Deletion

Because the Operator stores no per-user information on its own servers, deletion concerns the values stored on your device and the information held by third parties.

| Target | Retention | How to delete |
| --- | --- | --- |
| Game data stored on the device | Until you delete it | Web: clear this site’s stored data or `localStorage` in your browser / After app release: clear app data or uninstall the app |
| Hosting access logs | Per each hosting provider’s policy | Per the provider’s policy; the Operator does not identify users from these logs |
| Enquiry emails (sender address, subject, body, attachments) | 30 days after the enquiry is resolved | Deleted after the exchange ends. Where the law requires longer retention, kept only to the extent necessary for that period |

## 10. Your Rights and How to Exercise Them

You may exercise the rights below. For users covered by the GDPR or UK GDPR these include the rights of access, rectification, erasure (right to be forgotten), restriction of processing, data portability, objection, withdrawal of consent, and lodging a complaint with a supervisory authority. For users covered by U.S. state laws these include the rights to access, delete, correct, opt out of sale and sharing, and non-discrimination.

**How to exercise them**

- Game data stored on your device can be deleted directly using the methods in Section 9.
- For anything else, write to [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com). Where verification is needed we check the minimum information necessary and reply within 30 days of receipt (one month where the GDPR applies, extendable by two months with notice of the reason).
- The Operator runs no accounts, so an email address alone cannot locate a specific user’s device data. In that case deletion can only be completed with the device-side methods above.

**Supervisory authorities and dispute resolution**

- Republic of Korea: Privacy Infringement Report Centre https://privacy.kisa.or.kr (118) · Personal Information Dispute Mediation Committee https://www.kopico.go.kr (1833-6972) · National Police Agency cybercrime reporting https://ecrm.police.go.kr (182)
- EEA, United Kingdom, Switzerland: You may lodge a complaint with the data protection authority of your country of residence. See https://edpb.europa.eu/about-edpb/about-edpb/members_en for European authorities and https://ico.org.uk for the United Kingdom.

## 11. Children’s Privacy

The game is intended for users aged 13 and over and is neither designed nor operated primarily for children. Children are not asked to enter personal information, and no information is processed for child-directed advertising.

- Republic of Korea: A user under the age of 14 who needs to contact us must do so through a legal representative.
- EEA, United Kingdom: If you are under the digital consent age set by your country (13–16), a legal representative’s consent is required.
- United States: We do not knowingly collect personal information from children under 13. If we learn that we have, we delete it without delay.

## 12. Security Measures

- The game has no personal-data entry feature and the Operator runs no account system.
- Game data is stored only in device or browser storage and never copied to an Operator server.
- No dangerous or sensitive permissions are requested.
- All external communication uses HTTPS; plain HTTP is not used.
- No personally identifying information or device identifier is written to storage or logs.
- Before adopting a new SDK or network feature, permissions, consent flows and data flows are reviewed again.

## 13. Update Rules and Notice of Changes

If advertising, analytics, login, in-app purchases, cloud save, leaderboards, remote crash reporting, external server communication, a new distribution platform (Google Play, Apple App Store, Apps in Toss) or any other personal-data processing feature is added or changed, this policy and the privacy disclosures in each store or console are updated **before** the build containing that feature is released.

When this policy changes, the change and its effective date are announced on this page or in the service listing. As a rule, material changes to your rights are announced 30 days in advance and other changes 7 days in advance. **Corrections** that merely describe an already shipped feature accurately take effect immediately.

## 14. Contact and Effective Date

- Publisher name: LilyGames
- Operating entity: Lily S&C
- Privacy contact: [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com)

This policy is **effective from September 18, 2026**.

## Change History

- September 18, 2026: First edition, written for the web build which has no ads, no analytics and no server communication, and published on GitHub Pages. It states the on-device storage items (game progress, gold coins and items, daily reward record, volume and language settings), the hosting providers’ access logs, and your rights and deletion methods. The Korean edition was published at the same time.
