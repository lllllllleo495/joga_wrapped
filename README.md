# Yoga Wrapped Telegram Mini App

Interactive year-in-review experience for a Telegram bot that turns a user's yoga attendance history into animated, mobile-first visual stories.

> Portfolio-safe demo: all names, studio references, attendance data, and instructor images are synthetic and anonymized.

## Live Demo

Open the animated visualization:

[View Yoga Wrapped Demo](https://lllllllleo495.github.io/joga_wrapped/)

The demo is designed as a Telegram Mini App style story: progress segments, tap navigation, swipe gestures, hold-to-pause, animated counters, and share-ready summary slides.

## What The Bot Does

The original product flow:

1. A user starts analysis in Telegram.
2. The bot collects attendance history from a personal account.
3. The backend aggregates practice statistics without exposing other users' data.
4. The Mini App shows an animated personal Wrapped story.
5. After the story, the user can receive static cards in chat for social sharing.

## Product Highlights

- Telegram bot flow with `/start` and `/analyze`.
- Mobile-first Mini App visualization with story-like slides.
- Isolated per-user reports: each user sees only their own aggregate stats.
- Animated HTML/CSS/JS slides instead of static screenshots.
- Share-oriented final cards after the animated experience.
- Privacy-aware data model: demo uses synthetic data; production should avoid storing raw visit history longer than needed.

## Demo Features

- Animated slide progress with reliable back/forward state.
- Hold-to-pause behavior for reading dense slides.
- Responsive layout for phone and desktop.
- Instructor leaderboard, monthly rhythm, time-of-day analysis, class mix, and final recap.
- No real brand names, real instructor photos, phone numbers, tokens, or user data.

## Tech Stack

- Python Telegram Bot for conversational flow.
- Playwright for authenticated attendance collection.
- SQLite for latest aggregate Wrapped state.
- `aiohttp` web app for Telegram Mini App pages and secure callbacks.
- HTML, CSS, and vanilla JavaScript for animated story slides.
- Nginx + systemd deployment on VPS.

## Why It Matters

This project explores how a small Telegram bot can feel like a polished consumer product: personal, animated, privacy-aware, and easy to share. The work combines backend automation, data aggregation, deployment, and front-end storytelling in one end-to-end flow.

## Repository Notes

This public repository contains only a sanitized portfolio demo. Production secrets, real attendance exports, real instructor portraits, studio-specific copy, and deployment environment files are intentionally excluded.

