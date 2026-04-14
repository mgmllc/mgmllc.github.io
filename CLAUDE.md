# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is the GitHub Pages static website for MGM LLC (MGM合同会社), served at `mgm-llc.org`. It is a pure HTML/CSS site with no build system, package manager, or JavaScript framework.

## Site Structure

- `index.html` — Main landing page with company profile and Privacy Policy (English + Japanese).
- `apps/index.html` — App showcase page listing mobile apps published on App Store and Google Play.
- `assets/icons/` — App icon images (`bj-icon.png`, `baby-food-icon.png`, `kettou-icon.png`).
- `googled03fcaf1e003ff1c.html` — Google Search Console verification file (do not edit).
- `github_io.html` — Legacy/alternate page; not linked from main navigation.
- `CNAME` — Custom domain: `mgm-llc.org`.

## Apps Listed

| App | Android Package | iOS Status |
|-----|----------------|------------|
| Blackjack Absolute Counter | `com.mgm.blackjackabsolutecounter` | Live (`id1534572559`) |
| AI離乳食メーカー (AI Baby Food Maker) | `com.noriget.aibabyfoodmaker` | 準備中 (Coming soon) |
| AI血統診断 (AI Horse Racing Pedigree) | `com.mgm.aiKettouShindan` | 準備中 (Coming soon) |

## Conventions

- All CSS is inline within `<style>` tags in each HTML file — no external stylesheets.
- The site uses Apple-style design tokens (iOS blue `#007aff`, system font stack with `-apple-system`).
- Japanese text is used throughout for user-facing copy; English is used for company legal/policy sections.
- App Store badges are loaded from Apple/Google CDN URLs, not hosted locally.
- When an iOS app is not yet released, use a `<div class="store-status-placeholder">iOS版 準備中</div>` placeholder instead of the App Store badge.
- To add a new app card to `apps/index.html`, copy an existing `.app-card` div block, update the icon path under `/assets/icons/`, app name, description, and store links.
