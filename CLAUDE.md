# Readmigo Blog

## Project Overview

- **Type:** Hugo static blog
- **Theme:** PaperMod (git submodule)
- **Base URL:** https://blog.readmigo.app/
- **Site Title:** "Readmigo Blog"
- **Language:** English

## Deployment

- **CI/CD:** GitHub Actions → Cloudflare Pages (Wrangler)
- **Trigger:** Push to `main` branch, auto deploy (do NOT manually deploy)
- **Project name:** readmigo-blog

## Content Conventions

- Posts location: `content/posts/`
- File naming: lowercase with hyphens (e.g., `my-post-title.md`)
- Front matter format: **YAML** (not TOML, despite default archetype)

### Front Matter Template

```yaml
---
title: "Post Title"
date: YYYY-MM-DD
draft: false
tags: ["tag1", "tag2"]
categories: ["Category"]
summary: "Brief one-sentence summary"
---
```

### Writing Style

- Language: English
- Tone: Professional yet conversational, friendly and approachable
- Structure: Clear `##` and `###` headings, bullet points for features
- Short paragraphs (2-3 sentences)
- Focus: product value, AI capabilities, open-source philosophy

### Categories & Tags Used

- Categories: Product
- Tags: announcement, product, ai, english-learning, open-source, community

## Related Projects

- iOS app: `/Users/HONGBGU/Documents/readmigo-repos/ios`
- App name: Readmigo
- Bundle ID: `com.readmigo.app`
- App Store: https://apps.apple.com/app/readmigo/id6740539519

## iOS App Key Info (for blog reference)

### Version History

| Version | Date | Highlights |
|---------|------|------------|
| 2.0.0 | 2026-01-29 | Initial release |
| 2.0.1 | 2026-01-31 | Bug fixes (image loading, cache) |
| 2.0.2 | 2026-01-31 | UI improvements (bookstore structure) |
| 2.1.0 | 2026-02-02 | Multi-language support (11 languages) |
| 4.0.0 | 2026-02-11 | TTS/Audiobook/Analytics overhaul |

### Core Features

- AI-powered English reading companion
- 100,000+ free books (Project Gutenberg)
- 20,000+ free audiobooks (LibriVox)
- Text-to-Speech with cloud voices + sentence highlighting
- Audiobook player with bilingual reading mode
- Follow-along reading with speech recognition
- Vocabulary learning with spaced repetition
- AI author chat (voice, video, text)
- 11 language UI support
- PostHog analytics (v4.0+)

### 4 Main Tabs (v4.0)

1. Library
2. Discover
3. Audiobook (Listen) — new in 4.0, replaced Agora tab
4. Me

### Tech Stack

- Swift & SwiftUI, iOS 16.0+
- Kingfisher (image cache), GoogleSignIn, Sentry, PostHog
- MVVM architecture
