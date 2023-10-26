---
label: FAQ
icon: question
order: -98
---
# Frequently Asked Questions

## What is the behaviour when Marker collision occurs?

When there are Markers at the same timecode position, **Marker Data** will automatically resolve the collision of ID (Timecode, Name or Notes).

![Marker Collision](assets/fcp_marker_collision_01.png)

**Marker Data** will create unique Marker ID by automatically appending a numerical suffix at the end of the Marker ID and Image Filename.

![Unique Marker ID](assets/fcp_marker_collision_02.png)

![Unique Image Filename](assets/fcp_marker_collision_03.png)

## Does Marker Data replaces FCPXImageExporter?

Yes & No. Both **Marker Data** and **FCPXImageExporter** utilise different approach in solving a similar problem. **FCPXImageExporter** only extracts still images from source clips based on Makers. **FCPXImageExporter** completely ignores any post effects and titles applied to the timeline and individual clips. By contrast, Marker Data utilises both the output of the rendered timeline, and its accompanying FCPXML to derive all thumbnails (Stills or GIFs) and `.csv` to create a complete Data Set.

Comparison matrix between **Marker Data** and **FCPXImageExporter.**

Features   | Marker Data | FCPXImageExporter
:---:   | :---: | :---:
Speed | Moderate to Fast*  | Fast
Utilises Source Clips | No | Yes
Utilises Rendered Timeline  | Yes | No
RAW Files| Yes** | No
Effects, Titles & Transitions | Yes** | No
Creates .csv Data Set | Yes | No
Creates GIFs | Yes | No
Burn-Ins of Labels | Yes | No
Cost | Free & Open Source | Paid

**Dependent on your Mac’s hardware. With Apple Silicon, you can get faster results.*
***Rendered Timeline*

## Does Marker Data replaces Producer's Best Friend?

No. In fact it complements it. **Producer’s Best Friend** is the best application for creating spreadsheet report (for Numbers, Excel, Preview, etc.) about the Video Clips, Audio Clips, Titles, Generators, Markers, Keywords, Effects, and Transitions. **Marker Data** only extracts information pertaining markers and its accompanying metadata. Nothing more.

## Can Marker Data be used with other applications?

1. Yes. You can uncheck **Automatically Upload Converted FCPXMLs** in **Shot Data**’s Toolbox.
2. All Shot Data files are stored in **Export Destination** folder. Press **Reveal Export Destination** to open the folder.
3. In each sub folders, you will find the `*.csv` file with the accompanying images auto renamed.
4. You can import the `*.csv` to any application that accepts it.

## What is the appropriate workflow for naming VFX IDs?

Every project is different. But you can utilise this basic example.

``` VFX ID Example
XYZ701_150_010 - COOPER APPEARS NEAR PLANET SATURN
```

- **XYZ** is a 2-6 character code for the show or movie name
- **701** is a 3 digit episode number. For a standalone movie that is not episodic, any three digit number will suffice
- **150** is the scene number
- **010** is the shot number for the specific VFX shot within the scene
- **COOPER APPEARS NEAR PLANET SATURN** is the descriptive name of the shot

## Could Marker Data support DaVinci Resolve since it supports FCPXMLs?

No. Despite having the ability to import and export FCPXMLs from DaVinci Resolve, compatible Marker metadata is not added in the FCPXMLs.

## Why Notion v2 Token is used instead of Notion’s official API Connections?

Notion’s official API does not support direct upload and merging of images and page icons. It also does not support automatic linking or create new entries in relation columns based on their value. The day when Notion further opens up their APIs, we will look into updating our internal components.

Hence, Marker Data utilise [CSV2Notion Neo](https://github.com/TheAcharya/csv2notion-neo){target=“_blank”}.

## Will other database platforms be supported?

The current focus is to support and maintain Notion and Airtable integration. As these two are the most popular platforms among users and companies in the Film and TV industry. We took considerable amount of time in building our internal components for both Notion and Airtable.

In the database space, new platforms (both commercial and open-source) such as [Coda](https://coda.io/){target=“_blank”}, [Baserow](https://baserow.io/){target=“_blank”}, [AppFlowy](https://appflowy.io/){target=“_blank”}, Microsoft’s [Loop](https://loop.microsoft.com/learn){target=“_blank”} and the upcoming Google’s [Tables](https://www.youtube.com/@TablesfromArea120byGoogle/videos){target=“_blank”} are on the rise.

If you have a particular use case and platform in mind, please start a [discussion](https://github.com/TheAcharya/MarkerData/discussions){target=“_blank”}. However, the addition of platforms will be subjected to the availability of CLI or API libraries.

## Could Marker Data extract and convert Final Cut Pro's Marker metadata to another format?

Yes, it is possible. We will definitely add more [Profiles](https://github.com/TheAcharya/MarkersExtractor/issues?q=is%3Aissue+is%3Aopen+label%3Aprofiles){target=“_blank”} as we improve and update our API Library over time.

## Is Marker Data free to use?

Yes.

