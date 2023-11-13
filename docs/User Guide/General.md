---
label: General
icon: gear
order: -3
---
# General Settings

![General Settings](/assets/md-general-settings.png)

## Export Destination

### Destination

Click on the [!badge variant="success" text="Folder Icon"] to select your preferred location. 

You can click [!badge variant="success" text="Trash Icon"] to clear the stored path.

### Folder Format

[!badge variant="success" text="Folder Format"] allows you to select your preferred folder naming scheme. To prevent conflicts or overwrites of any previously generated files, both `Medium` and `Long` Folder Formats have `Current Date` and `Current Time` printed into naming scheme. Hence, every extraction is unique.

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

### Profiles

Select your desired Extraction Profile.
- **Notion** [!badge text="Default"]
- **Airtable**
- **MIDI**

### Exclude Roles

This a feature where you can exclude all the Marker metadata of data either `Video` or `Audio` Role.

### Enable Subframes

![Final Cut Pro's Time Display](/assets/fcp-subframes.png)

**Final Cut Pro** allows the user to view timecode at the subframe level.

!!!info Info
A subframe has 1/80 the duration of a video frame and is a more precise unit of reference when viewing or editing audio waveforms that are zoomed in to the sample level.
!!!

Checking [!badge variant="success" text="Enable Subframes"] will **Marker Data** to include the subframes in the `Marker ID`.

!!!info Info
[!badge variant="success" text="Enable Subframes"] will only work for `Timecode` under [!badge variant="success" text="Naming Mode"].
!!!

### Clip Boundaries

![Markers Within Clip Boundaries](/assets/fcp-clip-boundaries.gif)

When [!badge variant="success" text="Clip Boundaries"] is enabled, **Marker Data** will include Markers that are outside the bounds of a clip.

### No Media

By [!badge text="Default"] Marker Data will always look for accompanying movie file (`.mov` or `.mp4`) in directory where the `.fcpbundle` or `.fcpxml` resides. When [!badge variant="success" text="No Media"] is enabled, **Marker Data** will bypass the movie file.

This option is available in scenarios where :
- User do not have an output movie file.
- User does not wish to export movie file.
- User does not require image extraction.  
