---
label: General
icon: gear
order: -4
---
# General Settings

![General Settings](/assets/md-general-settings.png)

## Export Destination

### Destination

Select your desired location by clicking on the Folder Icon. Alternatively, the Trash Icon may be utilised to reset and clear the stored path.

### Folder Format

The Folder Format feature affords the user the capability to designate a folder naming scheme of their preference. In order to mitigate conflicts and potential overwrites of previously generated files, both the `Medium` and `Long` Folder Formats incorporate the inclusion of the `Current Date` and `Current Time` within the nomenclature. Consequently, each extraction yields a distinct and uniquely identified result.

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

### Enable Subframes

![Final Cut Pro's Time Display](/assets/fcp-subframes.png)

**Final Cut Pro** allows the user to view timecode at the subframe level.

!!!info Info
A subframe has 1/80 the duration of a video frame and is a more precise unit of reference when viewing or editing audio waveforms that are zoomed in to the sample level.
!!!

Checking Enable Subframes will **Marker Data** to include the subframes in the `Marker ID`.

!!!info Info
Enable Subframes will only work for `Timecode` under Naming Mode.
!!!

### Clip Boundaries

![Markers Within Clip Boundaries](/assets/fcp-clip-boundaries.gif)

When Clip Boundaries is enabled, **Marker Data** will include Markers that are outside the bounds of a clip.

### No Media

By [!badge text="Default"] Marker Data will always look for accompanying movie file (`.mov` or `.mp4`) in directory where the `.fcpbundle` or `.fcpxml` resides. Activating the No Media option allows **Marker Data** to circumvent the inclusion of the movie file during processing.

This option is available in scenarios where :
- User does not wish to export movie file.
- User does not require image extraction.  
