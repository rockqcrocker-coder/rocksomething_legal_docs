# Cookies & Local Storage Policy

**Rock Something**
**Effective Date:** [INSERT DATE]
**Last Updated:** [INSERT DATE]

---

## 1. Introduction

This policy explains how the Rock Something mobile application ("App") uses cookies, local storage, and similar technologies on your device. Because Rock Something is a native mobile app (not a website), our use of these technologies differs from typical web-based services.

## 2. Does the App Use Cookies?

**No.** Rock Something is a native mobile application and does not use browser cookies. The App does not place cookies on your device, and there are no third-party tracking cookies or advertising cookies.

## 3. Local Storage Technologies We Use

While we do not use cookies, the App does store a limited amount of data locally on your device for functionality purposes:

### 3.1 Secure Authentication Storage

| What | Purpose | Data Stored | Duration |
|------|---------|-------------|----------|
| **Auth Session Tokens** | Keep you signed in between app sessions | Encrypted authentication tokens (access token, refresh token) | Until you sign out or tokens expire |

- **Technology:** Expo Secure Store (uses iOS Keychain on Apple devices and Android Keystore on Android devices)
- **Encryption:** Data is encrypted by the operating system's secure storage mechanism
- **Size Limit:** Maximum 2048 bytes
- **Your Control:** Signing out of the App clears these tokens. You can also clear app data through your device settings.

### 3.2 Media Cache

| What | Purpose | Data Stored | Duration |
|------|---------|-------------|----------|
| **3D Model Frame Cache** | Faster loading of previously viewed 3D models | Downloaded GLB frame files | Temporary, cleared when app storage is cleared |
| **Video Frame Cache** | Faster video processing and playback | Extracted video frame data | Temporary, cleared when app storage is cleared |

- **Technology:** Expo File System (device local storage)
- **Purpose:** Performance optimization — avoids re-downloading content you've already viewed
- **Your Control:** You can clear the App's cache through your device settings (Settings > Apps > Rock Something > Clear Cache on Android, or offloading/deleting the app on iOS).

### 3.3 App State

| What | Purpose | Data Stored | Duration |
|------|---------|-------------|----------|
| **Navigation State** | Remember where you were in the App | Current screen/tab information | Current session only (in-memory) |
| **Form State** | Preserve form inputs while completing multi-step flows | Temporary form data (e.g., upload details, profile edits) | Current session only (in-memory) |

- **Technology:** In-memory state (React Native runtime)
- **Duration:** This data exists only while the App is running and is not persisted to disk

## 4. Third-Party Local Storage

### 4.1 Supabase Client
The Supabase authentication client stores session information using the secure storage mechanism described in Section 3.1. Supabase does not set additional cookies or tracking data on your device through the App.

### 4.2 No Third-Party Tracking
The App does not include any third-party analytics SDKs, advertising frameworks, or tracking pixels that would store data on your device.

## 5. What We Do NOT Store Locally

- No advertising identifiers or tracking cookies
- No browsing history or cross-app tracking data
- No third-party analytics data
- No fingerprinting data
- No social media tracking pixels

## 6. Web Views

If the App opens any web content (such as external links), the embedded web browser may use its own cookies and storage as determined by those websites. These are governed by the respective websites' privacy and cookie policies, not ours.

## 7. Your Choices

### 7.1 Clear App Data
You can clear all locally stored data at any time:
- **iOS:** Settings > General > iPhone Storage > Rock Something > Offload App (or Delete App)
- **Android:** Settings > Apps > Rock Something > Storage > Clear Cache / Clear Data

### 7.2 Sign Out
Signing out of the App removes your authentication tokens from secure storage.

### 7.3 Reinstall
Uninstalling and reinstalling the App removes all locally stored data, including cached content and authentication tokens.

## 8. Changes to This Policy

We may update this policy to reflect changes in our practices or for legal, operational, or regulatory reasons. We will update the "Last Updated" date and notify you through the App of any material changes.

## 9. Contact Us

If you have questions about this policy, contact us at:

**Email:** [INSERT CONTACT EMAIL]
**Website:** [INSERT WEBSITE URL]

---

*This Cookies & Local Storage Policy was last updated on [INSERT DATE].*
