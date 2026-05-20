---
title: Saige Privacy Policy
permalink: /saige/privacy/
---

# Privacy Policy — Saige

_Last updated: 20 May 2026_

Saige is a thinking-partner app where you chat with sixteen MBTI personality types. This page explains what data the app handles and where it goes.

## TL;DR

- **No account.** No sign-up, no login, no profile.
- **No analytics.** No tracking SDKs, no telemetry, no third-party trackers.
- **Conversations stay on your device.** Chat history and pinned facts are stored locally in an SQLite database inside the app's sandbox.
- **Messages you send are processed by Anthropic's Claude API** so the personalities can reply. They pass through our proxy server (a small Cloudflare Worker) and are not stored there.
- **Delete the app to delete everything.** Uninstalling removes the local database with all chat history and pinned facts.

## What we collect on your device

Stored locally only, in an SQLite database inside the app's sandbox:

- **Chat history** — your messages and the AI replies, grouped by personality.
- **Pinned facts** — things you've explicitly chosen for a personality to remember about you.
- **Identity preferences** — which fictional voice (e.g. Batman, Walter White) you've selected for each type.

This data never leaves your device unless you send a message that requires an AI reply (see below).

## What gets sent off your device

When you send a message:

1. The app forwards your message — plus the chat history for the active personality, plus any pinned facts you've added for them — to our **proxy server** at `saige-proxy.dtreg1.workers.dev`.
2. The proxy adds an API key and forwards the request to **Anthropic's Claude API** (`api.anthropic.com`).
3. Claude generates the reply and streams it back through the proxy to the app.

**The proxy is stateless.** It does not log, store, or retain the contents of any request after forwarding it.

**Anthropic processes the message** to generate the reply. Their data handling is governed by [Anthropic's Privacy Policy](https://www.anthropic.com/privacy) and [Usage Policy](https://www.anthropic.com/legal/aup). At the time of writing, Anthropic does not train on data sent via the API.

We do not associate any messages with you. There is no user ID, no device ID, no IP retention.

## Third parties

| Service | What it sees | Why |
| --- | --- | --- |
| Anthropic (Claude API) | The text of each message you send + the active personality's chat history + pinned facts | To generate the reply |
| Cloudflare Workers | Same as above, in transit only (not retained) | The proxy that holds the Anthropic API key |
| Apple (App Store) | Standard install / crash data | Required for App Store distribution |

We do not use Google Analytics, Firebase, Mixpanel, Segment, Sentry, or any other analytics or attribution SDK.

## Children

Saige is rated 12+. The app allows unrestricted prompts to a language model, so replies can in principle touch on any topic that conversations with adults might. We do not knowingly collect information from children under 13.

## Data retention

- **On your device:** indefinite, until you delete the app or clear chat history per personality from inside the app.
- **In transit:** the proxy does not retain anything after forwarding.
- **At Anthropic:** see their Privacy Policy. They retain API request logs for a limited time for abuse prevention, but do not train on API data.

## Your rights

- **Delete chat history** for a personality from inside the app (the personality detail screen).
- **Delete the app** to wipe everything.

You do not have an account on our servers, so there is nothing for us to delete on your behalf.

## Changes to this policy

If we change anything material, we'll update this page and bump the "Last updated" date at the top. If we ever start collecting analytics or building accounts, we'll require explicit opt-in.

## Contact

Email: dtreg1@gmail.com

For privacy or data-handling questions specifically related to Anthropic's processing, please also see [Anthropic's contact info](https://www.anthropic.com/privacy).
