# android-forensic-acquisition-adb

A streamlined toolkit and guide for performing live and dead forensic data acquisition from Android devices using the Android Debug Bridge (ADB). This project is designed for digital forensic investigators, incident responders, and security researchers to extract critical artifacts in a forensically sound manner.

---

## 📌 Features

* **Triage & Device Info:** Fast gathering of system properties, build details, and network configurations.
* **Live Artifact Extraction:** Comprehensive collection of running processes, installed packages, and active network connections.
* **File System Acquisition:** Targeted extraction of logical artifacts, databases, and logs without altering device integrity.
* **Automated Scripting:** Includes modular shell/batch scripts to automate sequential ADB commands and log outputs with cryptographic hashes.

---

## 🛡️ Forensic Best Practices Applied

1.  **Least Modification:** Commands are chosen to minimize writing to the target device's storage.
2.  **Chain of Custody & Integrity:** Generated acquisition logs automatically calculate SHA-256 hashes of the extracted data.
3.  **Documentation:** Every step, timestamp, and command execution is logged for reporting.

---

## 🚀 Getting Started

### Prerequisites

* **ADB (Android Debug Bridge):** Ensure the Android SDK Platform-Tools are installed and added to your system PATH.
* **Target Device Configuration:** USB Debugging must be enabled on the target Android device.

### Basic Usage

1. **Verify Connection:**
   Ensure your workstation recognizes the target device securely.
   ```bash
   adb devices
