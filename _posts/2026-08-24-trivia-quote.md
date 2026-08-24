---
layout: post
title: "Trivia Quote: A Daily Word, Quote & Trivia Game"
date: 2026-08-24 09:40
description: Trivia Quote is live on the App Store and Google Play — three daily brain games, weekly quizzes, streaks, and a monthly leaderboard, built with React Native, Expo, and Supabase.
tags: games mobile-dev react-native supabase side-project
categories: projects games
---

{% include figure.liquid path="assets/images/project_triviaquote/feature-graphic.jpg" class="img-fluid rounded z-depth-1" alt="Trivia Quote — three daily brain games: words, quotes, and trivia, from Clinkenbeard Games & Toys" %}

**Trivia Quote** is out and playable, on iOS and Android. It's the first title from **Clinkenbeard Games & Toys**, my small games label, and it's a daily habit-sized brain game: read a clue, pick the answer, and the faster you're right, the more you score.

> **Get it:** [App Store](https://apps.apple.com/app/id6797616680) · [Google Play](https://play.google.com/store/apps/details?id=com.cgandt.games.triviaquote) · [games.cgandt.com/triviaquote](https://games.cgandt.com/triviaquote)

## How it plays

Three modes, one fresh puzzle in each, every day:

- **Words** : a definition with four candidate words; pick the one it defines. Each word also carries a letter-based **tile score**, so rarer letters are worth more. _(It's a word game with a tile score — not affiliated with any other word/tile game.)_
- **Quotes** : a quote from a public-domain source: guess who said it.
- **Trivia** : a general-knowledge question spanning science, history, art, music, and more.

Every question is timed and scored speed-first, so answering fast and correctly is worth more than answering slow. Each mode wraps its week with a themed quiz drawn from that week's items, and the 1st of the month opens a free cross-mode "Month in Review" quiz built from the trickiest items of the previous month.

{% include figure.liquid path="assets/images/project_triviaquote/shot-question.jpg" class="img-fluid rounded z-depth-1" alt="A daily word puzzle: a definition with four word choices" caption="A fresh puzzle every day" width="240" %}
{% include figure.liquid path="assets/images/project_triviaquote/shot-answer.jpg" class="img-fluid rounded z-depth-1" alt="An answered quote question with the correct choice checked and its public-domain source linked" caption="Instant marking, sourced answers" width="240" %}

## Streaks, quizzes, and a board to climb

Streaks are tracked per mode, and correctness only counts the days you actually played — missing a day never tanks your percentage. The main leaderboard is a monthly board with a per-mode split (Words / Quotes / Trivia) plus the combined ranking, and Clinkenbeard Games & Toys members get their own private group board.

{% include figure.liquid path="assets/images/project_triviaquote/shot-quiz.jpg" class="img-fluid rounded z-depth-1" alt="A weekly quiz question with a four-dot progress row and the timer showing" caption="A weekly quiz in each mode" width="240" %}
{% include figure.liquid path="assets/images/project_triviaquote/shot-leaderboard.jpg" class="img-fluid rounded z-depth-1" alt="The monthly leaderboard with streaks and per-mode score breakdowns" caption="Climb the monthly board" width="240" %}

Play well and you unlock **hand-illustrated avatars** — Cartographer Fox, Astronomer Owl, Poet Raven, and more — each tied to a milestone like a 7-day streak.

{% include figure.liquid path="assets/images/project_triviaquote/shot-profile.jpg" class="img-fluid rounded z-depth-1" alt="The avatar collection: illustrated characters unlocked by playing, locked ones showing how to earn them" caption="Collect avatars as you play" width="240" %}

## How it's built

Trivia Quote is React Native on Expo, targeting Android and iOS from one codebase (web is a nice-to-have), with shared pure logic — scoring, timing, streaks — pulled into its own TypeScript `/core` package. The backend is Supabase: Postgres, Auth, and Edge Functions, with row-level security on every table so clients never write their own scores or entitlements. Timing is server-authoritative — the server issues a signed start token when a question opens and computes elapsed time on submit, so leaving the app to look something up only costs the speed bonus, and forged times get rejected.

The whole thing was built test-first: the scoring, timing, and entitlement logic in `/core` has exhaustive unit tests covering happy paths, timeouts, boundaries, and tampering, written before the implementation existed. No magic numbers either — every tunable (question time limit, speed-bonus curve, streak windows) is a named constant in one config module, not a number scattered through the code.

## What's next

Trivia Quote is in active development — paid tiers, an ad-supported free tier, monthly topic voting, and seasonal avatar drops are all on the roadmap. If you play it, [I'd love to hear what you think](mailto:drew@cgandt.com).
