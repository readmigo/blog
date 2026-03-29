---
title: "Readmigo 7.6.6: Smoother Sign-In, Pro Badges, and Web Upgrades"
date: 2026-03-29
draft: false
tags: ["announcement", "product", "update"]
categories: ["Product"]
summary: "A full-stack update across iOS, Android, and Web — region-adaptive sign-in, Pro subscription badges, new web pages, and a wave of stability fixes."
---

Version 7.6.6 is rolling out across all three platforms today. This release focuses on polishing the sign-in experience, giving Pro subscribers more visibility, and making the web app more complete.

## iOS: Region-Adaptive Sign-In

The sign-in screen now adapts to your region automatically. Depending on where you are, the app surfaces the most relevant login method as the primary button — so you see the option that makes the most sense for your location right away.

We've also added **phone number authentication** with a built-in country code picker. Select your country, enter your number, and you're in. This is especially useful in regions where email-based accounts are less common.

Under the hood, we improved how the app handles unexpected server responses. If the library API returns data in an unexpected format, the app now recovers gracefully instead of failing silently.

## Android: Pro Badge & Stability Fixes

Pro subscribers now get a **subscription badge on their profile card** — a gold border with a crown and PRO label. It's a small visual touch, but it makes your subscription status immediately visible.

This release also squashes several bugs:

- **Subscription status on first launch** — Previously, your Pro status might not show until you restarted the app. Fixed.
- **Purchase acknowledgment crash** — A JSON parsing edge case during purchase confirmation could cause a crash. Resolved.
- **Release build crash** — R8 code obfuscation was stripping classes it shouldn't have. Fixed with proper ProGuard rules.
- **Paywall back button** — The back button was slightly mispositioned. Now sits exactly where you'd expect it.

## Web: New Pages & Auth Stability

The web app at [web.readmigo.app](https://web.readmigo.app) gets several new pages and a round of important fixes.

**New features:**

- **Badge detail page** — Tap any badge to see how you earned it and what it represents.
- **Quote detail page & favorites** — Browse quotes from the books you're reading, and save your favorites for easy access.
- **Subscription settings page** — Manage your Pro subscription directly from the web, complete with a promo banner for free users.

**Stability improvements:**

- Fixed authentication issues where users could get stuck in redirect loops after signing in with Google.
- Improved middleware handling so protected routes work reliably even when session tokens are refreshed.
- Resolved a React rendering issue that could cause the profile page to crash under certain conditions.

## Get the Update

- [**App Store**](https://apps.apple.com/app/readmigo/id6740539519) (iOS)
- [**Google Play**](https://play.google.com/store/apps/details?id=com.readmigo.app) (Android)
- [**Web**](https://web.readmigo.app) (browser)

Happy reading.
