# 🎓 BIU Moodle Downloader

An unofficial, open-source Google Chrome extension designed to help Bar-Ilan University (BIU) students download course materials, recorded lectures, and entire folders in bulk with a single click. 

Instead of manually clicking through dozens of links and sub-folders, this extension automates the process, extracting the direct, unblocked URLs and sending them straight to your browser's download manager.

## ✨ Features
* **One-Click Bulk Download:** Scans the active Moodle course page and queues all available files.
* **Smart Folder Extraction:** Automatically navigates into Moodle folders (including complex nested sections) to retrieve the actual files.
* **Format Resolution:** Identifies and assigns the correct file extensions (.mp4, .pdf, .docx, .pptx) even when Moodle attempts to hide them.
* **Bypass Internal Viewers:** Forces Moodle to trigger a direct file download rather than opening documents inside the browser's internal PDF/Video viewer.
* **External Link Saving:** Captures external resource links and saves them as convenient `.txt` files so no material is lost.
* **Floating UI:** A clean, non-intrusive widget injected directly into the page with a real-time progress bar.

## 🚀 Installation (Developer Mode)
Since this extension is not listed on the Chrome Web Store, you will need to install it manually using Chrome's Developer Mode.

1. **Download the code:** Click the green `Code` button at the top of this repository and select **Download ZIP**. Extract the ZIP file to a folder on your computer.
2. **Open Extensions:** In Google Chrome, type `chrome://extensions/` into the address bar and press Enter.
3. **Enable Developer Mode:** Toggle the **Developer mode** switch in the top right corner of the screen.
4. **Load the Extension:** Click the **Load unpacked** button that appears in the top left.
5. Select the folder where you extracted the ZIP file. The extension will now appear in your browser!

## 📖 How to Use
1. Log in to the Bar-Ilan Moodle platform (`lemida.biu.ac.il`).
2. Navigate to the specific course page you want to download materials from.
3. Click the **BIU Moodle Downloader** icon in your Chrome toolbar (pin it for easy access).
4. A floating widget will appear at the bottom left of your screen. Click **Start Scan**.
5. The extension will scan the page and send the files to your download manager. Wait for the progress bar to reach 100%.

## ⚠️ Troubleshooting: Files Downloading as HTML (Bot Detection)
Occasionally, the university's anti-bot security system (Radware/ShieldSquare) might flag the extension's rapid download requests as automated bot activity. When this happens, your requested files (videos, PDFs, etc.) will incorrectly download as static HTML pages containing a security warning.

**How to resolve this:**
The system requires manual human verification to clear your session. To force this verification challenge:
1. Open your browser and navigate to any Moodle course page.
2. Aggressively refresh the page multiple times in a row (hold down `F5` or `Ctrl+R`). 
   *💡 Pro tip: Opening and rapidly refreshing several video lecture pages simultaneously is the fastest way to trigger the block.*
3. Within a few seconds, the Moodle platform should block your access and present an "I am not a robot" (hCaptcha) screen.
4. Solve the CAPTCHA challenge manually. 

Once you pass the verification, the security system will whitelist your session and grant you a "grace period" of several hours. You can then start the BIU Downloader extension and let it run freely without interruptions.

## ⚖️ Disclaimer
This is an unofficial, independent tool created by a student, for students, to optimize the learning process and save valuable time during exam periods. 

It is **not** affiliated with, endorsed by, or connected to Bar-Ilan University or its IT department. The extension runs entirely locally on your machine, utilizes your own active authentication session, and does not collect, store, or transmit any personal data. Users are expected to use this tool responsibly, ethically, and solely for their personal academic needs. Please be mindful not to intentionally overload the university's servers.
