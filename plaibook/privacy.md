---
title: PlAIbook Privacy Policy
permalink: /plaibook/privacy/
---

# Privacy Policy — PlAIbook

_Last updated: 20 May 2026_

PlAIbook ("we", "us", "the app") is a sports betting ticket tracker with AI-powered OCR, live score updates, and analytics. This policy describes what we collect, what we do with it, and the controls you have.

## 1. Who's running this

PlAIbook is operated by D. Trega ("we"). The app is distributed on the Apple App Store; the backend runs on a server we operate. We do not sell user data.

## 2. What we collect

When you use PlAIbook we store the following:

- **Account** — email address, name, and profile picture, provided by your OIDC identity provider (e.g., Google). We do not store passwords; authentication is delegated to the provider.
- **Betting tickets** — photos of tickets you scan, the AI-extracted ticket data (sport, event, selections, odds, stake), and the outcome (win/loss/push) once resolved.
- **Live score / event data** — we fetch live score and event status to determine ticket outcomes; we cache results against the events you've tracked.
- **Subscriptions** — your subscription tier, Stripe customer id, and current period state. Payment cards are handled by Stripe; we never see them.
- **Notifications** — push notification tokens if you opt in, used to alert you to ticket outcomes.

We do NOT collect: location, contacts, advertising id, biometric data, browsing history, or any third-party analytics SDKs.

## 3. How we use it

Solely to run the app:

- Authenticate you via your OIDC provider.
- Run OCR on ticket photos using Google's Gemini API to extract the structured ticket data.
- Generate AI-powered analytics, recommendations, and chat responses about your betting history, also via Gemini.
- Match your ticket selections against live score data to determine outcomes.
- Send push notifications about resolved tickets if you opt in.
- Process subscription events from Stripe and Apple App Store Server Notifications.

Tickets and their analyses stay scoped to your account. We do not use your data to train any AI model.

## 4. Third parties we share data with

- **Your OIDC provider** (Google, etc.) — handles authentication. They see your sign-in events; we receive your user id, email, name, and profile picture from them.
- **Google Gemini API** — receives ticket photos for OCR and ticket histories for analytics and chat. Subject to Google's API terms.
- **Stripe** — handles web-based subscription payments. Sees standard payment information; we never see your full card number.
- **Apple** — handles in-app subscription billing. Sees standard payment information; we never see your full card number.
- **Sports data providers** — we fetch live scores and event statuses from public sports data APIs. These services do not receive any user-identifying information.

Each of these is contracted as a processor: they process the data on our behalf, not for their own purposes.

## 5. How long we keep it

While your account is active, indefinitely — betting history loses its utility if we trim it, and analytics improve with more data points.

When you delete your account, we delete your personal data within 30 days. Ticket photos are deleted on the same schedule.

## 6. Your controls

- **Delete account** — contact us at [dtreg1@gmail.com](mailto:dtreg1@gmail.com) and we will fully delete your account and associated data within 30 days.
- **Cancel subscription** — via iOS Settings → Apple ID → Subscriptions (for App Store subs), or via your Stripe billing portal accessible from the web app (for web subs).
- **Disable notifications** — in iOS Settings → Notifications → PlAIbook, or in-app under Settings.

## 7. Responsible gaming

PlAIbook is a tracking and analytics tool. It does not facilitate betting; it does not place wagers; it does not partner with sportsbooks. If you or someone you know has a gambling problem, please contact the National Council on Problem Gambling at 1-800-522-4700 or [ncpgambling.org](https://www.ncpgambling.org/).

## 8. Children

PlAIbook is rated 17+ and is not intended for users under the legal gambling age in their jurisdiction. We do not knowingly collect information from anyone under 18.

## 9. Security

All traffic between the app and our backend is TLS. Database connections are TLS-only. Mobile bearer tokens are HMAC-signed and expire after 30 days. We have no employees other than the operator.

If we ever experience a breach that exposes user data, we will notify affected users within 72 hours of becoming aware of it.

## 10. Tracking

PlAIbook does not track you across other companies' apps or websites. We do not share your data with data brokers or use it for advertising.

## 11. CCPA / GDPR

California and EEA residents have the same rights described above — access, correction, deletion, export, and (for EEA) data portability and complaint to a supervisory authority. Email us to exercise any of these rights.

## 12. Changes to this policy

If we change anything material we'll update the "Last updated" date and notify you in-app the next time you open it. Non-material changes (typos, clarifications) may be made silently.

## 13. Contact

Email: [dtreg1@gmail.com](mailto:dtreg1@gmail.com)

We aim to respond within 7 days.
