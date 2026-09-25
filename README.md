# Packet Radio & Winlink EmComm Forms Suite

This suite provides a collection of 100% offline-ready HTML5 forms designed for Amateur Radio Emergency Communications (EmComm). They generate strictly formatted ASCII text blocks ready to be transmitted over AX.25 Packet Radio, VARA FM/HF, Winlink Express, or any terminal BBS.

## Key Features
* **Zero Dependencies:** Built with pure HTML, CSS, and vanilla JavaScript. No internet connection, server setup, or external libraries (like jQuery) are required.
* **Instant ASCII Generation:** Converts form inputs into 70-78 character word-wrapped, column-aligned ASCII text blocks formatted specifically for packet radio transmission.
* **Save as HTML:** Captures your active session (including text inputs, dropdown selections, checkboxes, and generated output) and exports a standalone `.html` file. This allows you to archive reports locally and re-open them later with all data intact.
* **One-Click Timestamps:** Instantly populate Date/Time fields in standard UTC (`HHMMZ`) or Local formats.

## Folder Structure & Included Forms
* **`general/`**
  * Winlink Check-In 
  * Net Control Check-In & Roster
  * General BBS Bulletin
  * Field Situation Report (FSR - 13 Lifelines)
  * TPRFN / RRI Digital Radiogram
  * ARRL Health & Welfare Radiogram
* **`ics/`**
  * ICS 205 (Radio Communications Plan)
  * ICS 213 (General Message)
  * ICS 214 (Activity Log)
  * Incident Status Report
  * Initial Damage Assessment (Windshield Survey)
* **`weather/`**
  * TPRFN Skywarn Winlink Generator
  * Current Local Surface Weather
  * Severe Weather Report (SKYWARN)
  * Hurricane Report (WX4NHC)

## How to Use

1. **Extract the Archive:** Unzip the suite to a designated folder on your computer, Toughbook, or field tablet.
2. **Open the Hub:** Double-click `index.html` to open the master dashboard in any modern web browser (Chrome, Firefox, Edge, Safari).
3. **Select a Form:** Click on any form card to launch it.
4. **Fill & Generate:** Enter your operational data and click **Generate Packet ASCII** at the bottom of the form. The formatted text will appear in the black terminal preview box.
5. **Copy to Terminal:** Click **Copy ASCII**. Switch to your packet client (e.g., Outpost Packet Message Manager, Winlink Express, SoundModem terminal, or PuTTY) and paste the text directly into the message body.
6. **Archive Your Work (Optional):** Click **Save as HTML**. A custom dialog box will prompt you for a filename (e.g., `FSR_Sector4_Update.html`). The browser will download a pristine copy of the form containing all your current data for offline record-keeping.

## Compatibility & Best Practices
* **Cross-Platform:** Works on Windows, macOS, Linux (including Raspberry Pi), Android, and iOS.
* **Local File Security:** Because these forms run locally via the `file:///` protocol, some browsers impose strict clipboard security. If the automatic clipboard copy is blocked, the script will automatically highlight the text for you—simply press `Ctrl+C` (or `Cmd+C`) to copy it manually.
* **Radiogram Strict Formatting:** The TPRFN/RRI generator automatically strips and converts standard punctuation (e.g., periods become `X`, dashes become `DASH`, `@` becomes `ATSIGN`) to adhere to strict NTS digital traffic handling rules.