---
title: "Readmigo 7.7.0: Badges, AI Translation, and a Smarter Reader"
date: 2026-04-05
draft: false
tags: ["announcement", "product", "update", "ai"]
categories: ["Product"]
summary: "A cross-platform update bringing a redesigned badge system, AI-first translation in the reader, word-boundary snapping, and 3D badges on Android."
---

Version 7.7.0 is here — across iOS, Android, and Web. This release introduces a redesigned badge system, smarter translation powered by AI, and a more precise reading experience.

## iOS: Badges Redesign & AI Translation

### Badges, Reimagined

The badge system gets a major overhaul. A new **My Badges** tab puts your earned badges front and center, sorted so unlocked ones always appear first. Each badge now shows clear unlock conditions, so you always know what to aim for next.

We've also added a **Level Benefits** view. Tap into any level to see the point rewards and decorative perks you unlock as you progress. A subtle chevron indicator makes the tap target obvious.

Behind the scenes, badge images now cache more reliably — pull-to-refresh clears stale thumbnails, and the cache integrates with the app's "Clear Cache" setting.

### AI-Powered Translation

The reader now defaults to **AI translation** when you highlight text. If pre-translated data is available, the app uses it instantly. If not, it falls back to real-time AI translation — no manual switching required.

A server-side kill switch lets us toggle this feature remotely, and the config caches for 24 hours to minimize network calls. We've also expanded translation event tracking to better understand how readers use this feature.

### Precise Word Selection

Drag handles in the reader now **snap to word boundaries**. When you adjust a text selection, the highlight locks to the nearest word edge instead of landing mid-character. It's a small change that makes selecting text noticeably more accurate.

## Android: 3D Badges & New Languages

Android catches up on the badge system with its own implementation, including a **3D badge engine** via JNI integration. You'll see badge capsules on your bookshelf, a full badge detail screen, medal notifications, and category tabs with a stats header and "next badge" advisor.

Translation gets a polish too — the translate button now pulses as a hint for new users, and we've added analytics events to track translation usage.

Two new languages join the roster: **Hebrew** and **Persian (Farsi)**, bringing our Android localization to 26 languages.

## Web: Community & Achievements

The web app at [web.readmigo.app](https://web.readmigo.app) adds two significant features:

- **Agora Community** — A new social space where you can browse posts, create your own, and leave comments on what others share.
- **Badges & Medals** — The achievement system arrives on web, so your reading milestones are visible wherever you log in.
- **Reading Analytics** — A new stats display with a weekly chart to track your reading habits over time.

## Get the Update

- [**App Store**](https://apps.apple.com/app/readmigo/id6740539519) (iOS)
- [**Google Play**](https://play.google.com/store/apps/details?id=com.readmigo.app) (Android)
- [**Web**](https://web.readmigo.app) (browser)

Happy reading.
