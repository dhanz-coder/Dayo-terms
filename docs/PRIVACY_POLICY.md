# PRIVACY POLICY

**Effective Date: April 25, 2026**
**Last Updated: April 25, 2026**

**Dayo** ("we," "us," "our," "the App") is operated from the Philippines. This Privacy Policy explains what information we collect, how we use and store it, who we share it with, and the choices and rights you have.

This policy complies with the **Data Privacy Act of 2012 (Republic Act No. 10173)** of the Philippines, the implementing rules of the National Privacy Commission (NPC), and Google Play's User Data policy.

---

## 1. WHO WE ARE

| Field | Value |
| --- | --- |
| App name | Dayo |
| Package name | com.dayo.google |
| Operator | Dayo (Philippines) |
| Data Privacy Officer | Dayo Data Privacy Officer |
| Privacy contact | privacy@dayo.ph |
| Support contact | support@dayo.ph |

---

## 2. INFORMATION WE COLLECT

### 2.1 Information you provide

**Account Information** (required to register)
- Full name
- Email address
- Mobile phone number
- Date of birth
- Password (stored only as a salted hash; we never see the plaintext)
- Authentication method used (email/password, Google, or Facebook)

**Profile Information** (optional)
- Profile photo
- Short bio / "About me"
- Gender
- City / province
- Preferred sport(s)

**Identity Verification** (optional, only if you choose to verify)
Verification is performed by **Persona** (Persona Identities, Inc., withpersona.com) inside the App. During verification Persona collects, **on its own servers**:
- A photo of your government-issued ID (driver's license, passport, national ID, voter's ID, student ID, etc.)
- A selfie used for face match
- Liveness detection signals
- OCR-extracted fields (ID number, name, date of birth, address)

Dayo **does not store the ID image, the selfie, or biometric templates**. From Persona we only receive and store: the verification result (approved / pending / declined), the type of document used, and a timestamp.

**Referee Profile** (only if you sign up as a referee)
- Sports certifications and uploaded certification documents
- Years of experience
- Rate per game
- Face photo for the public referee profile

**Content you create**
- Posts (text, photos, videos)
- Comments and reactions
- Direct messages and team-room chat messages
- Match results, scores, and statistics
- Club / community / team information you create or join
- Court bookings and challenge invitations
- Reports you file against other users or courts

**Payment & transaction data**
- Transaction history (platform fees, coin purchases)
- Reference numbers and amounts

We do **not** collect or store your full card number, CVV, GCash PIN, bank login, or any payment credential. Actual payment is processed by the third-party payment provider you choose (QR PH, and in the future GCash, GOtyme, Maya).

### 2.2 Information collected automatically

**Device & technical data**
- Device model, operating system and version
- App version
- Approximate IP address (used for security / abuse detection)
- Crash logs and error reports
- Push notification token (Firebase Cloud Messaging)

**Usage data**
- Which features and screens you use
- Frequency and time of use
- Interaction events used to improve the App

**Location data**
- **Precise GPS location** — accessed **only while you actively use** map-based features (finding nearby courts, viewing a venue on the map, getting directions, attaching a court to a booking).
- We do **not** collect background location.
- Your city/province from your profile is stored separately; precise GPS coordinates are used in real time and are not retained as a continuous location history.

**Camera, microphone, photos & media**
With your permission we access:
- Camera — for profile photos, ID verification, post photos and videos
- Microphone — only when you record a video for a post
- Photo / video library — for selecting media for posts or your profile

These are accessed only when you take the action that needs them.

### 2.3 Information from third parties

- **Google Sign-In** — name, email, profile photo, Google account ID
- **Facebook Login** — name, email, profile photo, Facebook account ID
- **Persona** — verification result and metadata (see 2.1)
- **Payment providers** — transaction reference, status, and amount

---

## 3. HOW WE USE YOUR INFORMATION

We use your information to:

1. **Provide the service** — create and maintain your account, show your profile, run matchmaking, deliver chat and notifications, run clubs and communities, accept court bookings, process platform-fee payments, calculate stats and ELO ratings.
2. **Authenticate and secure your account** — verify sign-in, prevent account takeover, detect fraud, spam and abuse.
3. **Communicate with you** — booking confirmations, match invites, team updates, important account or service notices.
4. **Verify identity (optional)** — process Persona verification results to issue verified badges and approve referees.
5. **Improve the App** — fix bugs, analyze usage patterns, plan new features.
6. **Enforce our Terms of Service and Community Guidelines** — review reports and take moderation actions.
7. **Comply with legal obligations** — respond to lawful requests, retain transaction records.

We do **not** use your data for personalized advertising. We do **not** sell your personal data.

---

## 4. HOW WE SHARE YOUR INFORMATION

### 4.1 What other Dayo users can see

**Visible to other users:**
- Your name, profile photo, bio, city/province
- Your verification badge (if any)
- Game stats, win/loss, ELO, club and community memberships
- Content you post publicly

**Never visible to other users:**
- Email address
- Phone number (unless you choose to share it in a chat)
- Date of birth
- Government IDs or biometric data
- Precise GPS coordinates

You can adjust some of this in **Profile → Privacy & Security** (profile visibility, online status, friend requests, game-history visibility).

### 4.2 Service providers we share with

| Provider | Data shared | Purpose | Location |
| --- | --- | --- | --- |
| **Supabase** (Supabase Inc.) | Account data, profile, posts, messages, media files, push token | Authentication, database, storage, realtime | Cloud (US / Asia-Pacific) |
| **Firebase Cloud Messaging** (Google LLC) | Push token, notification payload | Push notification delivery to your device | Google global infrastructure |
| **Persona** (Persona Identities, Inc.) | Government ID image, selfie, liveness, OCR fields | Identity verification (only if you opt in) | US / EU |
| **Mapbox** (Mapbox, Inc.) | Approximate / precise location while map is open | Map tiles and geocoding | US |
| **Google Sign-In** (Google LLC) | Google account profile when you sign in | OAuth authentication | Google global |
| **Facebook Login** (Meta Platforms, Inc.) | Facebook account profile when you sign in | OAuth authentication | Meta global |
| **QR PH / GCash / GOtyme / Maya** | Transaction amount and reference | Payment processing for platform fees | Philippines |

All providers process data under their own privacy policies and contractual data-protection commitments.

### 4.3 Legal disclosures

We may disclose your information when required by law: in response to a valid court order, subpoena, or government request; in cooperation with NPC investigations; to protect the rights, property, or safety of Dayo, our users, or the public; or to enforce our Terms of Service.

### 4.4 Business transfers

If Dayo is merged, acquired, or its assets are sold, your information may be transferred to the new owner. We will notify you in-app before such a transfer takes effect.

---

## 5. DATA STORAGE AND SECURITY

### 5.1 Where your data lives
- Account, profile, content, and messages: **Supabase** (PostgreSQL + Storage) in the US / Asia-Pacific region.
- Push delivery token: **Firebase Cloud Messaging**.
- ID verification artifacts: **Persona** (we do not hold these).

### 5.2 Security measures
- TLS / SSL for all data in transit
- AES-256 encryption at rest (provided by Supabase / Persona / FCM)
- Passwords stored as salted hashes — never in plaintext
- PKCE flow for OAuth sign-in
- Row-Level Security (RLS) on the database, restricting each user to their own rows
- Role-based access control for staff
- Limited, audited internal access for support and abuse investigations

While we follow industry-standard practices, no system is 100% secure. You are responsible for keeping your login credentials confidential.

### 5.3 Data retention

| Data | Retention |
| --- | --- |
| Account data | Until you delete the account, plus up to 30 days in encrypted backups |
| Posts, messages, chat history | Until you or we delete them |
| Verification result records | Up to 5 years (legal compliance) |
| Transaction records | 5 years (PH tax / accounting requirements) |
| Crash logs and analytics | Up to 12 months |
| Precise GPS coordinates | Used in real time, not stored as a history |

### 5.4 Data breach notification

In the event of a personal data breach that creates a real risk to you, we will:
1. Notify affected users within **72 hours** of confirmed discovery.
2. Notify the **National Privacy Commission** as required by RA 10173.
3. Provide guidance on protective steps you can take.

---

## 6. YOUR RIGHTS

Under the Data Privacy Act of 2012, you have the right to:

- **Access** — request a copy of the personal data we hold about you
- **Correction** — fix inaccurate data (you can do this directly in **Profile → Edit Profile**)
- **Erasure** — delete your account and personal data (**Profile → Privacy & Security → Delete Account**)
- **Object** — object to specific processing
- **Portability** — request your data in a structured, machine-readable format
- **Withdraw consent** — at any time, by deleting your account
- **Lodge a complaint** with the **National Privacy Commission** (info@privacy.gov.ph, https://www.privacy.gov.ph)

To exercise any right, email **privacy@dayo.ph**. We will respond within **15 days**.

### 6.1 Account deletion
You can permanently delete your account from the App at **Profile → Privacy & Security → Delete Account**. Deletion removes your personal data and content. Some records (transaction history, verification result, abuse reports) may be retained as required by law or to prevent fraud. Account deletion cannot be undone.

You can also request deletion outside the App by emailing **privacy@dayo.ph**.

---

## 7. CHILDREN'S PRIVACY

Dayo is intended for users **13 years of age and older**. Users **under 18 require verifiable parental or guardian consent**, which is collected in-app through the Parental Consent flow.

We do not knowingly collect personal data from children under 13. If you believe a child under 13 has created an account, contact **privacy@dayo.ph** and we will delete the account.

---

## 8. PERMISSIONS WE REQUEST

| Permission | Used for | Required? |
| --- | --- | --- |
| Camera | Profile photos, post photos/videos, ID verification | Optional |
| Photos / media library | Selecting photos and videos for posts and profile | Optional |
| Microphone | Recording audio in video posts | Optional |
| Precise location (foreground only) | Showing nearby courts, map view, attaching a venue to a booking | Optional |
| Notifications | Match invites, messages, team updates, booking confirmations | Optional |

Each permission is requested only when you first use the related feature. You can revoke any permission anytime from your device settings.

We do **not** request background location, contacts, SMS, call logs, or device files outside the photo library.

---

## 9. PUSH NOTIFICATIONS

We use Firebase Cloud Messaging (FCM) to deliver:
- Match invitations and team updates
- New messages
- Booking and payment confirmations
- Account or safety notices

You can disable notifications in **Profile → Settings → Notifications** or in your device settings.

---

## 10. INTERNATIONAL DATA TRANSFERS

Some service providers (Supabase, Google / FCM, Persona, Mapbox, Meta) process data outside the Philippines. Transfers are protected by:
- Contractual data-protection commitments with each provider
- Encryption in transit and at rest
- Compliance with the provider's certifications (SOC 2, ISO 27001, etc.)

By using Dayo you consent to these transfers.

---

## 11. AUTOMATED DECISION-MAKING

- **ELO rating** — automatically calculated from your match results.
- **Matchmaking suggestions** — based on skill level and approximate location.

These do not have legal or similarly significant effects on you. You can always decline a suggested match.

---

## 12. THIRD-PARTY LINKS AND SERVICES

The App may include links to third-party websites, courts, payment partners, or services. We are not responsible for their content or privacy practices. Please review their privacy policies before sharing data with them.

---

## 13. ADVERTISING AND TRACKING

Dayo does **not** display third-party advertisements, does **not** use advertising IDs, and does **not** share data with ad networks. We do not use cross-app tracking SDKs.

---

## 14. CHANGES TO THIS PRIVACY POLICY

We may update this Privacy Policy from time to time. When we make material changes we will:
- Show an in-app notice
- Email you (where we have an email on file)
- Update the "Last Updated" date at the top

Continued use of the App after the effective date of an update means you accept the updated policy.

---

## 15. CONTACT US

**Dayo — Data Privacy Officer**
Email: **privacy@dayo.ph**
Support: **support@dayo.ph**
Country: Philippines

**National Privacy Commission**
Email: info@privacy.gov.ph
Website: https://www.privacy.gov.ph

---

By creating an account and using Dayo you acknowledge that you have read and understood this Privacy Policy and consent to the collection, use, and sharing of your information as described.
