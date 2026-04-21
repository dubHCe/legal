---
layout: page
title: Privacy Policy
permalink: /privacy/
---

# Privacy Policy — Central Alerts

**Effective date:** April 21, 2026

This Privacy Policy describes how **Dubiel Hernandez Guerrero** ("we", "us", or "our")
collects, uses, stores, and shares information in connection with the
**Central Alerts** mobile application (the "App") and its backend service
("the Service"), together "Central Alerts".

Central Alerts is a business-to-business tool that delivers trading-related
event notifications from Best Contract Trader workstations to authorized
users on their mobile devices. The App is intended for use by adults (18+)
in a professional trading context.

If you have questions about this policy, contact us at
**support@bestcontrader.com**.

---

## 1. Information we collect

We collect only the information needed to operate the App and the Service.

### 1.1 Information you provide directly

- **Username and password** — used to authenticate you to the Service.
  Passwords are transmitted over an encrypted connection (HTTPS/TLS),
  hashed using PBKDF2-SHA256 with a random per-user salt and 600,000
  iterations, and the original password is never stored or logged.
- **Support requests** — when you use the "Report issue" feature, the text
  you type is transmitted to the Service and stored so that an administrator
  can respond.

### 1.2 Information the App collects automatically

- **Installation identifier** — a randomly generated unique identifier
  created the first time the App runs on your device. It is used to
  distinguish your device from other devices and is not tied to your
  personal identity.
- **Device platform and name** — whether the device is iOS or Android, and
  the device name configured in your operating system settings (e.g.,
  "Dubiel's iPhone"). Used to help you and administrators identify which
  device is which when multiple devices share an account.
- **Push notification token** — issued by Apple Push Notification service
  (APNs) or Firebase Cloud Messaging (FCM), this token allows the Service
  to deliver notifications to your device. It contains no personal data
  and is rotated by the operating system periodically.

### 1.3 Information the Service collects

- **Authentication tokens** — short-lived JSON Web Tokens (JWT) used to
  verify your identity on subsequent requests.
- **Event records** — alerts originating from trading workstations
  (severity, title, message, timestamps, associated metadata). These are
  the core content delivered by the App.
- **Notification delivery records** — which events have been delivered to
  you by email or push notification.
- **Device registration records** — the installation identifier, device
  name, platform, push token, and last-seen timestamp for each device
  registered to your account.
- **Read state** — which alerts you have opened, used only to mark alerts
  as read/unread in the App.

### 1.4 Information we do NOT collect

We do not collect, and the App does not have permission to access, any of
the following:

- Location data (GPS, approximate location, or otherwise)
- Contacts, photos, calendar, microphone, or camera
- Advertising identifiers or tracking identifiers for marketing
- Web browsing history outside the App
- Analytics or behavioral tracking
- Health, financial account, or payment information

The App does not use any third-party analytics, advertising, or marketing SDKs.

---

## 2. How we use your information

We use the information we collect solely to:

1. Authenticate you to the Service and keep your session secure.
2. Deliver event notifications to the correct users and devices.
3. Display alert history, read/unread state, and related information in
   the App.
4. Respond to support requests you submit through the App.
5. Diagnose and resolve technical problems.
6. Comply with legal obligations.

We do not use your information for advertising, profiling, automated
decision-making, or sale to third parties.

---

## 3. How we share your information

We share information only in the following limited circumstances:

- **Service providers that make the App function.** Specifically:
  - **Google / Firebase Cloud Messaging** — receives the notification
    payload (title, body, alert ID) in order to deliver push notifications
    to your Android device. Google's privacy policy:
    <https://policies.google.com/privacy>
  - **Apple Push Notification Service (APNs)** — receives the same type of
    notification payload in order to deliver push notifications to your
    iOS device. Apple's privacy policy:
    <https://www.apple.com/legal/privacy/>
  - **Cloudflare, Inc.** — our hosting partner for the Service, which
    provides TLS encryption and traffic routing. Cloudflare processes
    requests transiently and does not retain application content.
    Cloudflare's privacy policy:
    <https://www.cloudflare.com/privacypolicy/>
  - **Email service providers** — used to send event-summary emails and
    support-response emails to addresses you or your administrator have
    configured. The specific provider is described in account-setup
    documentation and may change over time.

- **If required by law.** We may share information when compelled by a
  valid subpoena, court order, or similar legal process, or to prevent
  imminent harm.

- **Internal administrators.** Users with administrator privileges within
  your organization can view events, device registrations, and support
  requests within their scope of responsibility, as part of operating the
  Service for your organization.

We do not sell personal information. We do not share information with
advertisers or data brokers.

---

## 4. Where your information is stored

- **On your device.** Authentication tokens, the installation identifier,
  and your selected workstation preference are stored in the operating
  system's secure storage (Keychain on iOS, Keystore-backed
  EncryptedSharedPreferences on Android). Read-state and language
  preferences are stored in standard app preferences.
- **On our servers.** Account records, events, and device registrations
  are stored in a PostgreSQL database hosted on infrastructure under our
  control in the United States.

---

## 5. How long we keep your information

- **Account information** is retained for as long as your account is active.
- **Authentication tokens** expire automatically within 30 minutes and are
  not retained after expiration.
- **Events and notification delivery records** are currently retained
  indefinitely in the Service database. We are implementing a scheduled
  retention policy that will automatically delete records older than a
  specified age.
- **Support requests and administrator responses** are retained
  indefinitely to preserve conversation history.
- **Device registrations** are retained until you unregister the device
  (sign out and remove the App) or an administrator removes it.

You may at any time request that we delete your account and associated data
(see Section 7).

---

## 6. Security

We take reasonable measures to protect your information:

- All network traffic between the App and the Service is encrypted using
  TLS (HTTPS). The App does not connect to the Service over unencrypted
  HTTP in production.
- Passwords are never stored in plaintext. They are hashed using PBKDF2-
  SHA256 with per-user random salts and 600,000 iterations before storage.
- Authentication tokens are short-lived and signed with a server-side
  secret that is rotated periodically.
- Device storage of tokens uses the operating system's secure storage
  primitives (iOS Keychain / Android Keystore).
- Server infrastructure is access-controlled and audited.

No system is perfectly secure. If we become aware of a security incident
that affects your information, we will notify affected users as required
by applicable law.

---

## 7. Your rights and choices

You can:

- **Access, correct, or delete your account data.** Contact us at
  **support@bestcontrader.com** to request a copy of the personal information
  we hold about you, or to ask us to correct or delete it.
- **Unregister a device.** Signing out of the App within a device unlinks
  that device from your account and stops push notifications to it.
- **Disable push notifications.** Use your device's Settings app → Central
  Alerts → Notifications to turn off push notifications without signing out.
- **Close your account.** Request that we permanently delete your account.
  We will complete such requests within 30 days of verification.

---

## 8. Children's privacy

Central Alerts is not intended for users under the age of 18. We do not
knowingly collect information from anyone under 13 (in compliance with the
Children's Online Privacy Protection Act, "COPPA"). If you believe a child
under 13 has provided us with personal information, contact us at
**support@bestcontrader.com** and we will delete it.

---

## 9. California residents

If you are a resident of California, you have the following rights under
the California Consumer Privacy Act (CCPA):

- The right to know what personal information we have collected about you.
- The right to request deletion of your personal information.
- The right to not be discriminated against for exercising these rights.

We do not sell personal information, so there is no "opt out of sale"
process to invoke. To exercise any of the rights above, contact
**support@bestcontrader.com**.

---

## 10. Changes to this policy

We may update this Privacy Policy from time to time. When we do, we will
update the effective date at the top of this page. For material changes,
we will also notify active users through the App before the changes take
effect. Your continued use of the App after changes become effective
constitutes acceptance of the revised policy.

---

## 11. Governing law

This Privacy Policy is governed by the laws of the State of Florida,
United States, without regard to its conflict-of-laws provisions.

---

## 12. Contact us

If you have questions, concerns, or requests about this policy or your
personal information:

**Dubiel Hernandez Guerrero**
Email: **support@bestcontrader.com**

---

*This policy was last updated on April 21, 2026.*
