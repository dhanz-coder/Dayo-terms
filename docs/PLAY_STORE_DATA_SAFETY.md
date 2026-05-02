# Play Store Data Safety Form — Dayo

This is a copy-paste reference for the **Data safety** section in the Google Play Console (App content → Data safety). Answers reflect the actual Dayo codebase as of April 25, 2026.

---

## Section 1 — Data collection and security (overview)

| Question | Answer |
| --- | --- |
| Does your app collect or share any of the required user data types? | **Yes** |
| Is all of the user data collected by your app encrypted in transit? | **Yes** (TLS to Supabase, FCM, Persona, Mapbox, OAuth providers) |
| Do you provide a way for users to request that their data be deleted? | **Yes** — in-app at *Profile → Privacy & Security → Delete Account*, and by email at privacy@dayo.ph |

---

## Section 2 — Data types

For every entry below: mark **Collected = Yes**, **Shared = No** (unless noted), **Processed ephemerally = No** (unless noted), **Required or optional** as listed, **Purpose** as listed.

> "Shared" in Play Console means transferred to a *third party*. Sending data to your own backend (Supabase) is **collection**, not sharing. Sending to FCM, Persona, Mapbox, Google/Facebook OAuth, and payment providers is **sharing** because those are independent third parties.

### Personal info

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| Name | Yes | No | Required | Account management, App functionality |
| Email address | Yes | No | Required | Account management, Communications |
| User IDs | Yes | No | Required | Account management, App functionality, Fraud prevention/security |
| Address | No | — | — | — |
| Phone number | Yes | No | Required | Account management, Fraud prevention/security |
| Race and ethnicity | No | — | — | — |
| Political or religious beliefs | No | — | — | — |
| Sexual orientation | No | — | — | — |
| Other info (date of birth, gender, bio, sport preference, city/province) | Yes | No | Optional (DOB is required for age check) | Account management, Personalization, App functionality |

### Financial info

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| User payment info (full PAN/card) | No | — | — | — |
| Purchase history (transactions, coin purchases, platform fees) | Yes | Yes — to payment providers (QR PH / GCash / GOtyme / Maya) | Optional | App functionality, Fraud prevention/security, Compliance |
| Credit score / other financial info | No | — | — | — |

### Health and fitness

> Match results / ELO are **gameplay** data, not health data. Do **not** declare Health & fitness.

### Messages

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| Emails | No | — | — | — |
| SMS or MMS | No | — | — | — |
| Other in-app messages (DMs, team-room chat) | Yes | No | Optional | App functionality |

### Photos and videos

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| Photos | Yes | No | Optional | App functionality (profile, posts), Account management |
| Videos | Yes | No | Optional | App functionality (posts) |

### Audio files

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| Voice or sound recordings | If you keep RECORD_AUDIO: Yes (audio recorded with video posts). Otherwise: **remove the permission and answer No.** | No | Optional | App functionality |
| Music files | No | — | — | — |
| Other audio files | No | — | — | — |

### Files and docs

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| Files and docs (referee certifications, ID documents) | Yes — referee certs uploaded to Supabase Storage; ID documents go to **Persona, not Dayo** | Yes — to Persona for verification | Optional | App functionality (Account management for verification) |

### Calendar / Contacts

Both **No**.

### Location

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| Approximate location | Yes (derived from GPS, only when map is open) | Yes — to Mapbox to fetch tiles/geocode | Optional | App functionality |
| Precise location | Yes (foreground only, only when map is open) | Yes — to Mapbox | Optional | App functionality |

> Important: declare location as **collected and shared with Mapbox**. Mapbox is a third party.

### Web browsing

**No**.

### App activity

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| App interactions (taps, screens visited, feature usage) | Yes | No | Optional | Analytics, App functionality |
| In-app search history | No | — | — | — |
| Installed apps | No | — | — | — |
| Other user-generated content (posts, comments, reactions, reports, club/community/team data, match results) | Yes | No | Optional | App functionality |
| Other actions | No | — | — | — |

### App info and performance

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| Crash logs | Yes | No | Required | App functionality, Analytics |
| Diagnostics (device model, OS version, app version) | Yes | No | Required | App functionality, Analytics |
| Other app performance data | Yes | No | Required | App functionality |

### Device or other IDs

| Data type | Collected | Shared | Required/Optional | Purposes |
| --- | --- | --- | --- | --- |
| Device or other IDs (FCM push token, install ID) | Yes | Yes — push token shared with Firebase Cloud Messaging (Google) | Required | App functionality (notifications), Fraud prevention/security |

---

## Section 3 — Security practices (questions Play asks)

| Question | Answer |
| --- | --- |
| Is your data encrypted in transit? | **Yes** |
| Do you have a way for users to request data deletion? | **Yes — in-app and via privacy@dayo.ph** |
| Have you committed to following the Play Families Policy? | **Only if you target users under 13.** Dayo's minimum age is 13, so answer "No" unless your store listing says otherwise. |
| Has your app been independently security-reviewed against MASVS? | **No** (unless you've actually done it) |

---

## Section 4 — Permissions declarations the listing must explain

Play Console requires a justification for these. Use the strings below.

| Permission | Justification text (paste into Play Console) |
| --- | --- |
| `ACCESS_FINE_LOCATION` / `ACCESS_COARSE_LOCATION` | Used **only in the foreground** to display your position on the map, find courts near you, and attach a venue to a court booking. Not used in the background. |
| `CAMERA` | Used to take a profile photo, capture photos and videos for posts, and for in-App identity verification handled by Persona. |
| `RECORD_AUDIO` | Used to capture audio when the user records a video post. **If unused, remove from the manifest.** |
| `READ_MEDIA_IMAGES` / `READ_MEDIA_VIDEO` | Used to let the user pick existing photos and videos from their library to attach to posts or set as a profile photo. |
| `READ_MEDIA_AUDIO` | **Likely unused — remove unless a feature actually picks audio files.** |
| `POST_NOTIFICATIONS` | Required to deliver match invites, new messages, team updates, and booking confirmations via push. |
| `SYSTEM_ALERT_WINDOW` | **Likely not needed and Play Store flags this. Remove unless you have a specific overlay feature.** |

---

## Section 5 — Other Play Console items you must complete

- **Target audience and content** — declare ages 13+ and verify you collect verifiable parental consent for users under 18.
- **Ads** — answer **"No, my app does not contain ads."**
- **Government apps** — No.
- **Financial features** — declare **"In-app purchases"** (coin purchases) and "Payments inside the app" if you process platform fees through QR PH/GCash/etc.
- **Health** — No.
- **News** — No.
- **COVID-19 contact tracing** — No.
- **Data privacy & security policy URL** — host the contents of `docs/PRIVACY_POLICY.md` on a public URL (e.g. https://dayo.ph/privacy) and paste it here. Play **rejects** apps where this URL is missing, returns 404, or doesn't actually describe your data practices.

---

## Section 6 — Action items before you submit

1. Decide whether `RECORD_AUDIO`, `READ_MEDIA_AUDIO`, and `SYSTEM_ALERT_WINDOW` are actually used. Remove from `android/app/src/main/AndroidManifest.xml` and `app.json` if not — every extra permission triggers more Play Store review questions.
2. Host the Privacy Policy at a stable HTTPS URL **before** filling the Data Safety form (Play Console requires the URL there, not just inside the app).
3. Make sure the **email addresses** in the policy (`privacy@dayo.ph`, `support@dayo.ph`) actually receive mail — Play reviewers send test emails.
4. Confirm the in-app **Account Deletion** flow at `Profile → Privacy & Security → Delete Account` actually works end-to-end. Google now also requires a **web-based** deletion request URL (https://dayo.ph/delete-account or similar) since 2024.
5. Verify the **age gate**: registration must reject users < 13 and trigger parental consent flow for 13–17.
6. Update the in-app `PrivacyPolicyScreen.tsx` "Last Updated" date and the contact email so they match this document.
