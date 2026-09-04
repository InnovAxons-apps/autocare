# Privacy Policy for AutoCare

**Effective Date:** September 5, 2026  
**Last Updated:** September 5, 2026  
**Publisher:** InnovAxons (`com.innovaxons.autocare`)  
**Contact:** innovaxons.apps@gmail.com  

---

## 1. Introduction & Core Philosophy

AutoCare ("the Application") is developed and maintained by **InnovAxons**. We believe your private vehicle records, maintenance history, driving habits, and financial logs belong exclusively to you. 

AutoCare is engineered from the ground up on an **Offline-First, Data-Sovereign Architecture**. We do not operate developer tracking servers, we do not require account registration, and we do not collect, sell, monetize, or harvest your personal information.

---

## 2. Information We Do NOT Collect

Because AutoCare operates without a proprietary backend server:
* **No Account Credentials:** You are not required to create an account, log in, or provide your name, phone number, or password to use AutoCare.
* **No Analytics or Telemetry:** The Application contains no third-party tracking libraries, advertising SDKs, behavioral analytics, or marketing pixels.
* **No Vehicle Telematics Harvesting:** Your odometer readings, maintenance intervals, vehicle identification numbers (VIN), fuel fill-up records, and expenses remain strictly inside your device's secure local sandbox.

---

## 3. Information Stored Locally on Your Device

All Application data is stored locally in an offline SQLite database and within the private sandbox storage directory allocated to AutoCare by your mobile operating system (Android / iOS):
* **Vehicle Profiles:** Make, model, year, trim, license plate, color, and odometer readings.
* **Service & Maintenance Logs:** Completed services, parts replaced, costs, notes, and service dates.
* **Document & Glovebox Records:** Expiration dates and metadata for vehicle registration, insurance, and inspections.
* **Locally Attached Photos:** Receipt snapshots, document scans, and vehicle avatar images.

This data never leaves your physical device unless you explicitly initiate an external backup.

---

## 4. Device Permissions & Why They Are Needed

AutoCare requests only the minimal system permissions necessary to deliver its core vehicle tracking utilities:

| Permission | Platform | Purpose |
| :--- | :--- | :--- |
| **Camera** | Android / iOS | Enables you to take photos of paper workshop receipts, invoices, and vehicle registration cards directly within the app. Images are stored locally on your device. |
| **Photo Library / Storage** | Android / iOS | Enables you to select and attach existing photos of receipts, invoices, or vehicle images to your service logs. |
| **Notifications** | Android / iOS | Used strictly to schedule **local offline reminders** on your device when a maintenance interval is due or when an insurance/registration document is nearing its expiration date. No remote notification server is contacted. |
| **Internet Access** | Android / iOS | Used exclusively when you explicitly choose to connect and synchronize your backups with your personal Google Drive account. |

> [!NOTE]
> AutoCare **does not** access your microphone, contacts, location, audio recordings, or biometric hardware.

---

## 5. Cloud Backup & Data Synchronization (User-Controlled)

AutoCare provides optional, user-directed cloud backup options:

### A. Google Drive Synchronization (Android / Cross-Platform)
* **User-Initiated:** Google Drive synchronization is strictly optional and disabled by default.
* **Direct Transfer:** When you choose to link Google Drive, authentication is handled directly between your device and Google using OAuth 2.0.
* **Narrow Scope (`drive.file`):** AutoCare requests only the restricted `https://www.googleapis.com/auth/drive.file` scope. This technical boundary guarantees that AutoCare can **only access and modify files that it specifically created** (its own backup archive). AutoCare cannot see, read, or alter any other files, photos, or documents in your Google Drive.
* **Zero Intermediaries:** Your backup data travels encrypted directly between your device and Google's servers. No data ever passes through or touches an InnovAxons server.

### B. Apple iCloud Synchronization (iOS)
* When operating on iOS devices, synchronization leverages Apple's native iCloud sandbox storage associated with your personal Apple ID.

### C. Manual Local Backup & Restore
* You can export a complete, unencrypted JSON backup of your garage records and receipts to your local storage or files app at any time, allowing you full control and portability of your data.

---

## 6. Data Retention & Deletion

You maintain complete sovereignty over your data:
* **In-App Reset:** You can delete individual vehicles, service items, or your entire database directly through the **Settings > Reset All Data** option inside the app.
* **Uninstalling the App:** Uninstalling AutoCare from your device automatically purges all locally stored records, databases, thumbnails, and cache from your device storage.
* **Cloud Backup Deletion:** You can delete your Google Drive or iCloud backup archives at any time by unlinking the provider in Settings or directly deleting the backup folder inside your personal cloud storage.

---

## 7. Children's Privacy

AutoCare does not target, collect, or solicit information from anyone under the age of 13 (or applicable age in your jurisdiction). The Application is a general-purpose vehicle management utility.

---

## 8. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect new app features, updated operating system permissions, or regulatory requirements. Any modifications will be posted with an updated "Effective Date" at the top of this document.

---

## 9. Contact Us

If you have questions, concerns, or feedback regarding this Privacy Policy or AutoCare's data privacy design, please contact us:

* **Developer:** InnovAxons
* **Email:** innovaxons.apps@gmail.com
* **Official Webpage:** https://innovaxons.github.io/autocare/
