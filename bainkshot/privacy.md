---
title: BainkShot Privacy Policy
permalink: /bainkshot/privacy/
---

# Privacy Policy — BainkShot

_Last updated: 21 May 2026 (rev. 2)_

BainkShot ("we", "us", "the app") is a financial forecasting and tax-prep tool for individuals and small businesses. This policy describes what we collect, what we do with it, and the controls you have.

## 1. Who's running this

BainkShot is operated by D. Trega ("we"). The app is distributed on the Apple App Store; the backend runs on a server we operate. We do not sell user data.

## 2. What we collect

When you use BainkShot we store the following:

- **Account** — your email address, name, and (if you upload one) profile photo, via Clerk authentication. Passwords are managed by Clerk; we never see them.
- **Financial transactions** — every statement transaction you import (CSV, spreadsheet, or pasted data), including date, description, amount, account, and our derived category. This is the primary purpose of the app and is required for it to work.
- **Receipts** — any receipt images or PDFs you attach to a transaction, stored in Google Cloud Storage scoped to your user id.
- **Tax profile** — entity type, deductions, mileage logs, business expenses, and any tax-related fields you enter for the current tax year.
- **Subscription status** — your plan tier and Apple transaction id linking your purchase. Payment cards are handled by Apple; we never see them.

We do NOT collect: location, contacts, advertising id, biometric data, browsing history, or any third-party analytics SDKs.

## 3. How we use it

Solely to run the app:

- Authenticate you against your account (via Clerk).
- Show you your transactions, categories, and tax rollups.
- Run AI categorization on transactions you've imported, by sending the transaction descriptions to OpenAI's API. OpenAI does not train on data sent via the API.
- Run AI tax-document parsing on documents you upload, by sending the document text to OpenAI's API.
- Process App Store subscription events through Apple's App Store Server Notifications so we can keep your tier accurate.

We do not use your data to train any AI model, our own or third-party.

## 4. Third parties we share data with

- **Clerk** — handles authentication. They see your email, password (hashed), name, and profile photo.
- **OpenAI** — receives transaction descriptions for categorization and document text for parsing. Subject to OpenAI's API terms; prompts are not used for model training.
- **Google Cloud Storage** — stores receipt images and PDFs you upload. Files are scoped to your user id in the bucket path.
- **Apple** — subscription state, transaction id, original transaction id, auto-renew flag.

Each of these is contracted as a processor: they process the data on our behalf, not for their own purposes.

## 5. How long we keep it

While your account is active, indefinitely — financial records lose their utility if we trim them, and tax-prep often requires multi-year lookback.

When you delete your account, we delete your personal data within 30 days. Receipt files in Google Cloud Storage are deleted on the same schedule.

## 6. Your controls

- **Delete account** — contact us at [dtreg1@gmail.com](mailto:dtreg1@gmail.com) and we will fully delete your account and associated data within 30 days.
- **Export** — download a **Tax Folio** workbook (Excel `.xlsx`) containing your transactions, categorized rollups, and receipts list for the current tax year. On web: from the **Tax Center** page. On the mobile app: from the **Tax** tab, which opens your device share sheet so you can save the file to Files, send it via Mail, etc.
- **Cancel subscription** — via iOS Settings → Apple ID → Subscriptions. Apple handles cancellation and prorating; we do not have access to your payment instrument.

## 7. Children

BainkShot is not intended for users under 18. We do not knowingly collect personal information from anyone under 13.

## 8. Security

All traffic between the app and our backend is TLS. Receipts in GCS are encrypted at rest by Google. Database connections are TLS-only. We have no employees other than the operator.

If we ever experience a breach that exposes user data, we will notify affected users within 72 hours of becoming aware of it.

## 9. Tracking

BainkShot does not track you across other companies' apps or websites. We do not share your data with data brokers or use it for advertising.

## 10. CCPA / GDPR

California and EEA residents have the same rights described above — access, correction, deletion, export, and (for EEA) data portability and complaint to a supervisory authority. Email us to exercise any of these rights.

## 11. Changes to this policy

If we change anything material we'll update the "Last updated" date and notify you in-app the next time you open it. Non-material changes (typos, clarifications) may be made silently.

## 12. Contact

Email: [dtreg1@gmail.com](mailto:dtreg1@gmail.com)

We aim to respond within 7 days.
