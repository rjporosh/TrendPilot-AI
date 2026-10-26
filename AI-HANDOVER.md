# TrendPilot AI — AI Handover

## Project

TrendPilot AI creates original Bengali short videos and manages publishing across YouTube, Facebook and Instagram.

## Owner's Goal

The owner wants a system that can research relevant topics, create AI visuals and Bengali narration, publish regularly and optimize future content from analytics.

## Environment

macOS / MacBook Pro. Preferred stack: Python, FFmpeg, SQLite and optional n8n.

## Important Unknown

The owner has a reported one-billion-token allowance but has not confirmed the exact provider. Never guess the service or request API secrets. Ask for its exact name or redacted documentation. Use a generic adapter and mock provider until confirmed.

## Mandatory Rules

* Official OAuth and publishing APIs only.
* Never request social passwords.
* Social URLs alone do not authorize publishing.
* Approval-required mode by default.
* Enable public automation only after successful tests.
* Track usage rights for every asset.
* Block critical safety and rights failures.
* Prevent duplicate posts.
* Enforce budgets, upload caps and emergency stop.
* No fake engagement, copied videos or monetization promises.

## Working Instructions

Inspect the repository before editing. Build a runnable vertical slice first. Run tests and fix failures. Clearly report which features are implemented, mocked, unverified or blocked by external account requirements. Keep secrets out of Git. Update release notes and this handover after substantial changes.

## Current Status

This document describes requirements and intended architecture. It does not claim that the full application or live platform integrations already exist.
