# TrendPilot AI — Master Specification

## Product Vision

Build a Python-first AI content studio that researches relevant topics, creates original Bengali short videos, publishes them to YouTube Shorts, Facebook Reels and Instagram Reels through official APIs, and learns from available analytics.

## Core Features

1. Secure account connections using official OAuth.
2. Trend research from permitted public sources and owned-channel analytics.
3. Multiple-niche experimentation and transparent idea scoring.
4. Original Bengali script and storyboard generation.
5. AI-generated visuals, Bengali narration, captions and FFmpeg rendering.
6. Copyright, asset-license, quality, factuality and synthetic-media disclosure checks.
7. Official YouTube Data API and Meta Graph API integrations.
8. Publishing calendar, retries, duplicate prevention and job tracking.
9. Analytics dashboard for views, retention where available, engagement, audience growth and reported revenue where accessible.
10. Budget limits, provider-usage tracking, audit logs and emergency stop.

## Architecture

* Python application with modular services.
* FastAPI backend and responsive dashboard.
* SQLite for local MVP, with migrations.
* Pluggable LLM, visual-generation and Bengali TTS providers.
* FFmpeg for rendering.
* Official publishing adapters for YouTube and Meta.
* Python scheduler initially; optional n8n orchestration later.
* Mock mode for development without credentials.

## Publishing Rules

* Approval-required mode is the default.
* Enable automated public publishing only after successful integration and safety tests.
* Social profile links alone do not authorize publishing.
* Never request or store social account passwords.
* Use official OAuth and minimum required permissions.
* Never bypass API restrictions, rate limits or platform policies.
* Prevent duplicate uploads and stop on critical rights or quality failures.

## Security

* Store secrets outside source control.
* Protect and securely store OAuth tokens.
* Never log API keys or tokens.
* Provide disconnect, pause and recovery controls.
* Record asset sources, usage rights and commercial-use permissions.

## Monetization

The system must never promise guaranteed views, monetization or income. It should display eligibility guidance and official account status where available. Originality and platform policy compliance are mandatory.

## Acceptance Criteria

* Clean installation works on macOS.
* Demo mode works without external credentials.
* A sample original vertical MP4 can be rendered.
* Dry-run publishing makes no live API calls.
* Missing rights evidence blocks publishing.
* API failures are handled without duplicate uploads.
* Daily budgets and emergency stop work.
* Tests pass and documentation accurately identifies mocked and unverified integrations.

## Unresolved Configuration

The exact AI provider behind the user's reported one-billion-token allowance must be confirmed before selecting its SDK. Visual-generation provider, Bengali TTS provider, account permissions, budget and hosting plan also require confirmation.
