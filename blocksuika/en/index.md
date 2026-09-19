---
layout: default
title: Gem Maker Privacy Policy
description: Gem Maker device storage, shared leaderboard, ads, analytics and privacy rights.
permalink: /blocksuika/en/
---

# Gem Maker Privacy Policy

[한국어](../)

- First published: September 18, 2026
- Updated/effective: September 20, 2026, for builds containing the leaderboard feature
- Developer: Lilygames / Operator: LilySnC
- Contact: [lilygames@lilysnc.com](mailto:lilygames@lilysnc.com)
- Website: https://lilygames.lilysnc.com
- Service: Gem Maker (formerly BlockSuika)

## 1. Scope

This policy covers Gem Maker for web, Google Play, App Store and Apps in Toss. Actual processing depends on the platform and installed build. The previous statements that the service has no server, identifiers or leaderboard have changed with the shared leaderboard.

## 2. Device storage

We store game progress, best score, play counts, coins/items, daily rewards, spins, ad usage counters, discovered gems, item-help acknowledgements, language and audio settings on the device. Web uses localStorage; native apps use app-specific storage; Apps in Toss uses SDK storage. The complete game save is not uploaded to the leaderboard server. Coins are in-game currency and cannot be exchanged for cash. A password or real name is not required to play.

## 3. Shared leaderboard

When enabled, the app contacts our server at startup to create or restore a device-local anonymous participant and authentication session. The server stores an opaque participant ID and a hash of a recovery credential. The device stores that credential; short-lived access tokens are held in runtime memory. This restores the participant on the same installation but does not automatically link installations on different devices or platforms.

**Public registration is optional.** On a new best, the app displays the nickname and score and requests your agreement before sending them. An existing local best is offered separately on the home screen. A cancelled draft is not automatically submitted. Your last confirmed nickname and an approved unfinished request may be stored locally for restoration and retry.

Submission data includes nickname, score, participant ID, rules version, request/result identifiers and nickname revision. Public rankings show nickname, score, rank and opaque participant information. **Do not put your real name or contact information in a nickname.** Credentials and access tokens are not published.

Gem Maker has separate leaderboard data from Steelball. IP addresses are processed for request limiting and security and may appear in proxy/server access logs. Leaderboard scores are not used as evidence for cash or promotional payouts.

## 4. Ads, analytics and promotions

- Web currently simulates rewarded-ad buttons without playing external ads and does not compose Firebase Analytics. Leaderboard API communication is separate.
- Google Play/iOS code includes AdMob and Firebase Analytics integration. Where configured, providers may process advertising IDs, IP-derived approximate location, device/app information, ad interactions and diagnostics/analytics. Builds without configured iOS ad units do not display ads.
- Apps in Toss uses Toss SDK ads and platform event processing. Preapproval test builds use test ad IDs. Promotion codes are currently pending values with zero payout amounts, so actual promotional grants are disabled.

Provider policies and applicable platform/regional settings apply. The game does not require location, contacts, photos, camera or microphone permission for ranking registration.

## 5. Purposes and choices

Device saves provide gameplay continuity. Anonymous credentials authenticate and restore participants. Request limits protect the service from abuse. Your optional publication of a nickname and score provides rankings. Applicable legal bases include service performance, your agreement to public registration, and legitimate security interests where recognized by law.

You can decline public registration and continue playing. Audio and language settings are available in the game. Consult device and provider settings for available advertising choices.

## 6. Service providers and processing locations

| Provider | Role |
|---|---|
| Cloudflare | Web hosting, public HTTPS API proxy, security and access logs |
| Oracle Cloud | Hosting our separate leaderboard API and database |
| GitHub | Hosting this privacy policy |
| Google | AdMob/Firebase in applicable native builds and support email |
| Toss | Apps in Toss storage, ads and platform features |

Providers may process information across their global infrastructure. Locations, retention and transfer safeguards depend on their policies, applicable contracts and law. Clients use the public HTTPS API. The current Cloudflare-to-origin proxy connection uses HTTP; it is not described as end-to-end TLS.

[Cloudflare](https://www.cloudflare.com/privacypolicy/) · [Oracle](https://www.oracle.com/legal/privacy/) · [Google](https://policies.google.com/privacy) · [GitHub](https://docs.github.com/site-policy/privacy-policies/github-general-privacy-statement)

## 7. Retention, deletion and recovery

Device data remains until you clear the site/app data. Server rankings do not have automatic expiry and are retained while providing the service or until a deletion request is processed. Session tokens are valid for 24 hours; request-limit records expire according to their windows. Provider logs and backups follow their applicable operating policies. Support email is deleted within 30 days after resolution unless longer retention is legally required.

**Clearing device data or uninstalling the app does not automatically delete a published server ranking.** Contact lilygames@lilysnc.com to request access, correction, deletion or withdrawal of publication consent. We will explain the minimum verification needed, such as nickname and participant identification. Do not email passwords, recovery credentials or access tokens. If an anonymous credential is lost, an email address alone may not establish ownership or restore the record.

## 8. Your rights and children

Subject to applicable law, you may request access, correction, deletion, restriction, portability, object to processing or withdraw consent. Send requests to the contact above; applicable statutory response periods apply. You may also contact your local privacy authority, including Korea's privacy reporting center (118) or dispute mediation commission.

The game targets users aged 13 and over and is not primarily directed to children. Users below the applicable local consent age must obtain any required guardian consent. We take appropriate removal measures when unnecessary children's personal information is identified.

## 9. Security and changes

Server signing secrets are not included in the game bundle. Recovery credentials are hashed server-side. We validate request size, frequency and input and separate public rankings from credentials. These measures do not prove that a client-submitted score reflects genuine gameplay. We do not sell personal information.

When features or processing change, we update this policy and required store disclosures. We provide notices and obtain any consent required by applicable law.

## Changes

- September 20, 2026: Shared anonymous leaderboard, optional nickname/score publication, authentication/recovery data, server retention/deletion and platform ad/analytics status.
- September 18, 2026: Initial publication and Gem Maker naming update.
