---
label: Release Notes
icon: note
order: -98
---
# Release Notes

### 1.3.0 (11)

**🎉 Released:**
- 8th July 2025

**🔨 Improvements:**
- Added new **Compressor Chapters** Profile
- Added new **Markdown List** Profile

<hr>

### 1.2.3 (10)

**🎉 Released:**
- 26th June 2025

**🔨 Improvements:**
- Updated Notion Module CSV2Notion Neo to version 1.3.6

**🐞 Bug Fix:**
- Fixed an issue in the Notion module that was preventing Marker Data's Data Set from being uploaded

<hr>

### 1.2.2 (9)

**🎉 Released:**
- 21st June 2025

**🔨 Improvements:**
- Updated Pagemaker Module to version 1.1.0
- Pagemaker module now includes a new `PDF Compression` dialog box - Click the `Gear` icon to reveal a compression slider with four levels – `None`, `Low`, `Medium`, and `High`
- Pagemaker module now features a significantly enhanced the image compression algorithm for `Export PDF`
- Pagemaker module now supports emojis in Marker Data’s extracted data sets, leveraging the [Unicode Emoji JSON](https://github.com/muan/unicode-emoji-json) database
- Pagemaker module now automatically converts emojis to descriptive text during PDF export – For example, `🔥 Metaburner` becomes `[fire] Metaburner`
- Pagemaker module now displays gallery cards with a black background for improved visual clarity and contrast

<hr>

### 1.2.1 (8)

**🎉 Released:**
- 15th June 2025

**🔨 Improvements:**
- Updated Pagemaker Module to version 1.0.7
- Pagemaker module now maintains aspect ratios for vertical images in PDF exports, ensuring parity with gallery preview

<hr>

### 1.2.0 (7)

**🎉 Released:**
- 12th May 2025

**Marker Data** no longer officially supports macOS Ventura starting with version 1.2.0.

**🔨 Improvements:**
- Introducing [Pagemaker](/user-guide/pagemaker/) – a new feature that allows users to create PDFs directly within Marker Data
- Swatch analysis now provides percentage progress, including completion status for each processed image
- Updated Notion Module CSV2Notion Neo to version 1.3.5
- Increased Notion Module's upload threads

<hr>

### 1.1.4 (6)

**🎉 Released:**
- 29th March 2025

**🐞 Bug Fix:**
- Removed unintended exposure of the XML Path column in certain Extraction Profile

<hr>

### 1.1.3 (5)

**🎉 Released:**
- 20th February 2025

**🔨 Improvements:**
- Updated [Troubleshooting](troubleshooting.md) guide to include Module Status

**🐞 Bug Fix:**
- Fixed a critical bug that caused Marker Data's Workflow Extension to crash in macOS Sequoia

<hr>

### 1.1.2 (4)

**🎉 Released:**
- 17th February 2025

**🔨 Improvements:**
- Updated Notion Module CSV2Notion Neo to version 1.3.4
- Updated Workflow Extensions SDK to 1.0.3
- Internal dependencies updates
- Codebase updates for Xcode 16.2
- Complete codebase updates and refactors for Swift 6 strict concurrency compatibility

**🐞 Bug Fix:**
- Fixed a critical bug in the Notion module that prevented Marker Data's Data Set uploads due to Notion API changes
- Markers placed on transitions are now extracted correctly
- YouTube Chapters Extraction Profile now formats output timestamps consistently formatted as `HH:MM:SS`
- YouTube Chapters Extraction Profile now inserts initial chapter marker at `00:00:00` if one does not exist

<hr>

### 1.1.1 (3)

**🎉 Released:**
- 14th November 2024

**Marker Data** is now exclusively build and optimised for Apple Silicon only.

**🔨 Improvements:**
- Added support and compatibility for FCPXML v1.13 (Final Cut Pro 11)
- Added support and compatibility for frame rates `90p`, `100p` and `120p`

<hr>

### 1.1.0 (2)

**🎉 Released:**
- 11th November 2024

**Marker Data** is now exclusively build and optimised for Apple Silicon only.

**🔨 Improvements:**
- Application bundle size has been reduced
- User can now Assign Shortcut to Configurations
- Codebase updates for better compatibility with Xcode 16
- Updated Notion Module CSV2Notion Neo to version 1.3.3
- Updated Airtable Module Airlift to version 1.1.4

**🐞 Bug Fix:**
- Fixed a critical bug in the Notion module that prevented Marker Data's Data Set uploads when Notion Database URL is not provided

<hr>

### 1.0.0 (1)

**🎉 Released:**
- 11th July 2024

This is the first public release of **Marker Data**!

-![](https://i.giphy.com/Lp71UWmAAeJHi.webp)