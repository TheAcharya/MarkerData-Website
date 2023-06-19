---
label: General
icon: gear
order: -3
---
# General Settings

## Export Destination

### Select Location

### Folder Format

## Extraction Profile

### Profiles

Select your desired Extraction Profile.
- **Notion** [!badge text="Default"]
- **Airtable**
- **MIDI**

### Exclude Roles

This a feature where you can exclude all the Marker metadata of data either **Video** or **Audio** Role.

### Enable Subframes

![Final Cut Pro's Time Display](/assets/fcp-subframes.png)

**Final Cut Pro** allows the user to view timecode at the subframe level. A subframe has 1/80 the duration of a video frame and is a more precise unit of reference when viewing or editing audio waveforms that are zoomed in to the sample level.

Checking **Enable Subframes** will **Marker Data** to include the subframes in the `Marker ID`.

!!!info Info
Enabling subframes will only work when **Naming Mode** is in **Timecode** Mode.
!!!

### Clip Boundaries

![Markers Within Clip Boundaries](/assets/fcp-clip-boundaries.gif)

When **Clip Boundaries** is enabled, **Marker Data** will include Markers that are outside the bounds of a clip.

### No Media

By [!badge text="Default"] Marker Data will always look for accompanying movie file (`.mov` or `.mp4`) in directory where the `.fcpbundle` or `.fcpxml` resides. When **No Media** is enabled, **Marker Data** will bypass the movie file.

This option is available in scenarios where :
- User do not have an output movie file.
- User does not wish to export movie file.
- User does not require image extraction.  
