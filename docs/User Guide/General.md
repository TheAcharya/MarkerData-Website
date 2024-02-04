---
label: General
icon: gear
order: -4
---
# General Settings

![General Settings](/assets/md-general-settings.png)

## Export Destination

### Destination

You can select your desired location by clicking on the Folder Icon. Upon right-clicking folder icon, **Marker Data** will show the `Full Path` associated with said folder.

### Folder Format

The Folder Format feature allows you the capability to designate a folder naming scheme of your preference. In order to mitigate conflicts and potential overwrites of previously generated files, both the `Medium` and `Long` Folder Formats incorporate the inclusion of the `Current Date` and `Current Time` within the nomenclature. Consequently, each extraction yields a distinct and uniquely identified result.

Select your desired Folder Format.
- **Short**
- **Medium** [!badge text="Default"]
- **Long**

!!!info Info
Short
`Marker Data Demo_V1`

Medium
`Marker Data Demo_V1 2023-03-21 09-45-22`

Long
`Marker Data Demo_V1 2023-03-21 09-45-22 [Notion]`
!!!

## Extraction Profile

![Extraction Profiles](/assets/md-general-settings-extraction-profile.png)

### Profiles

Select your desired Extraction Profile.

- Extract Only (No Upload)
	- **CSV** [!badge text="Default"]
	- **TSV**
	- **MIDI**
	- **Notion (No Upload)**
	- **Airtable (No Upload)**
- Database Profiles (Upload)
	- When you create a [Database Profile](/user-guide/databases), it will be listed here.

### Enable Subframes

![Final Cut Pro's Time Display](/assets/fcp-subframes.png)

**Final Cut Pro** allows the you to view timecode at the subframe level.

!!!info Info
A subframe has 1/80 the duration of a video frame and is a more precise unit of reference when viewing or editing audio waveforms that are zoomed in to the sample level.
!!!

Checking Enable Subframes will **Marker Data** to include the subframes in the `Marker ID`.

!!!info Info
Enable Subframes will only work for `Timecode` under Naming Mode.
!!!

### No Media

By [!badge text="Default"] Marker Data will always look for accompanying movie file (`.mov` or `.mp4`) in directory where the `.fcpxmld` or `.fcpxml` resides. Activating the No Media option allows **Marker Data** to circumvent the inclusion of the movie file during processing.

This option is applicable in situations wherein:

- You do not require exporting a movie file.
- You do not require extraction of images.

<hr>

## Progress Reporting

![](/assets/md-general-settings-notifications.png)

### Notification Frequency

**Marker Data** seamlessly integrates with the native macOS Notifications framework, delivering timely alerts upon the successful completion of tasks.

Select your desired Notification Frequency.
- **Never**
- **Only on Completion** [!badge text="Default"]
- **All Steps**

### Show Progress on Dock Icon

By [!badge text="Default"] Progress Bar is shown on **Marker Data**'s dock icon.

### Open macOS Notification Settings

![](/assets/md-general-settings-notifications_macOS.png)

Select the `Open macOS Notification Settings` link to open macOS Notification Settings. Navigate to **Marker Data** to manage notification settings.

!!!info Info
**Marker Data** will only show up in the macOS Notification Settings solely after the initial prompting attempt. If **Marker Data** is the focused application, notifications won’t make a sound or appear on the screen.
!!!

<hr>

## Roles

![](/assets/md-general-settings-roles.png)