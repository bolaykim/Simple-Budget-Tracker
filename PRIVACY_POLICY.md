# Privacy Policy for Simple Budget Tracker

**Effective Date:** November 22, 2026  
**Last Updated:** November 22, 2026  
**App Package:** `com.simplebudgettracker_v1`  
**Developer:** Simple Series  

Simple Budget Tracker ("the App") is designed to be a minimalist, privacy-first personal finance tool. We respect your privacy and built the App so that **all of your financial data stays strictly on your device**.

---

## 1. Data Collection & Storage

**We do not collect, transmit, sell, or share any of your personal or financial data.**

- **100% Local Storage:** All budgets, expenses, income entries, categories, savings goals, and app preferences are stored exclusively on your device using local storage (`localStorage` and Android `SharedPreferences` for the home screen widget).
- **No Accounts & No Cloud Servers:** The App does not require registration, login, or an internet connection to function, and we do not operate any backend servers that receive your data.
- **No Analytics or Advertising:** The App does not include third-party analytics SDKs, ad networks, or tracking libraries.

---

## 2. Optional Notification Auto-Capture (`NotificationListenerService`)

Simple Budget Tracker offers an **optional, user-enabled** feature called **Payment Notification Auto-Capture** to help you quickly log expenses and income from payment apps (such as Google Wallet, Samsung Pay, PayPal, Revolut, Wise, or banking apps).

If you choose to enable this feature and grant **Notification Access** (`BIND_NOTIFICATION_LISTENER_SERVICE`):

- **What is read:** The App inspects incoming notifications on your device solely to detect payment or refund amounts and estimate an expense/income category (e.g., Food, Groceries, Transport) based on keywords.
- **100% On-Device Processing:** All notification parsing happens strictly in memory on your device. Raw notification text is **never uploaded, transmitted over the internet, or shared with any third party**.
- **Minimal Data Retention:** Raw notification text is discarded immediately after parsing. Only the resulting transaction amount, type (expense/income), guessed category, and timestamp are saved locally—either automatically (in *Auto-Log* mode) or only after you tap to confirm (in *1-Tap Confirm* mode).
- **Full User Control:** This feature is **disabled by default**. You can choose which payment app categories to monitor, switch between *1-Tap Confirm* and *Auto-Log* modes, or revoke Notification Access at any time in your Android device settings (*Settings → Notifications → Notification access*).

---

## 3. Permissions Used

The App requests only the permissions needed for its features:

- **Notification Access (`BIND_NOTIFICATION_LISTENER_SERVICE`) — Optional:** Used solely for on-device detection of payment notifications when you opt in to Payment Auto-Capture.
- **Post Notifications (`POST_NOTIFICATIONS`) — Optional:** Used on Android 13+ to show local confirmation or auto-logged alerts when a payment notification is detected.
- **Vibrate (`VIBRATE`):** Used for tactile haptic feedback when interacting with the App.
- **Internet (`INTERNET`):** Required by Android's WebView container and used only if you voluntarily tap external links (such as the optional "Buy Me a Coffee" support link). The App does not transmit your budget data over the internet.

---

## 4. Backups, Exports & External Links

- **Manual Export / Share:** You may export your budget data as a JSON backup file or share a formatted text summary using your device's standard share sheet. Any file or text you choose to export or share is handled under your direct control.
- **Android System Backup:** The App supports Android's standard Auto Backup (`android:allowBackup="true"`), which may back up local app data to your personal Google account if you have Google Device Backup enabled in Android settings. We have no access to these backups.
- **External Links:** The Settings screen includes an optional link to PayPal to support the developer. If you tap this link, it opens in your device's browser and is governed by PayPal's own Privacy Policy.

---

## 5. Data Deletion

Because all data is stored locally on your device, you have complete control over deleting it at any time:

- Delete individual entries or reset your data within the App's Settings.
- Clear the App's data via Android *Settings → Apps → Simple Budget Tracker → Storage → Clear data*.
- Uninstall the App from your device to permanently remove all local data.

---

## 6. Children's Privacy

Simple Budget Tracker does not knowingly collect any personal information from anyone, including children under the age of 13 (or the applicable age of digital consent in your jurisdiction).

---

## 7. Changes to This Privacy Policy

We may update this Privacy Policy from time to time if we add new features or to reflect changes in legal or platform requirements. Any updates will be posted at this URL with an updated "Last Updated" date.

---

## 8. Contact Us

If you have any questions or concerns about this Privacy Policy or the App's data practices, please contact us at:

- **Developer:** Simple Series
- **Email:** eren.hursit@hotmail.com
