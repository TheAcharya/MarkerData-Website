---
label: FAQ
icon: question
order: -96
---
# Frequently Asked Questions

## What behavioural outcomes manifest in the event of Marker collision?

In instances where Markers coincide, **Marker Data** will adeptly rectify any conflicts arising from overlapping Marker ID such as Timecode, Name, or Notes.

![Marker Collision](assets/fcp_marker_collision_01.png)

**Marker Data** will create unique Marker IDs through an automated process of appending a numerical suffix to both the Marker ID and the Image Filename.

![Unique Marker ID](assets/fcp_marker_collision_02.png)

![Unique Image Filename](assets/fcp_marker_collision_03.png)

## What behavioural intricacies arise when Markers are situated within a Compound, Multicam and synchronised clips?

**Marker Data** is intentionally configured to disregard any markers outside the primary active timeline. This deliberate choice is particularly pertinent in scenarios involving Compound Clips, where the potential for numerous nested structures exists. Parsing markers within each nested Compound Clip could introduce undue complexity.

Should a user wish to extract markers from within a Compound Clip, a straightforward approach involves double-clicking the specific Compound Clip and exporting its associated timeline. In doing so, any markers nested within that particular Compound Clip's timeline will be excluded from consideration by **Marker Data**.

## What behavioural outcomes manifest in the event when Markers are intentionally obscured by trimmed clips?"

![Obscured Markers](assets/fcp-obscured-markers.gif)

Employing a WYSIWYG methodology, Marker Data adopts an automated process wherein markers obscured within the timeline due to trimmed clips are inherently excluded.

## To what extent does Marker Data supersede the functionality of FCPXImageExporter?

Indeed, there are distinctions between the methodologies employed by **Marker Data** and **FCPXImageExporter** in addressing analogous challenges. **FCPXImageExporter** singularly focuses on the extraction of static images from source clips delineated by markers. This process, however, intentionally overlooks any post-effects and titles applied at both the timeline and individual clip levels.

In contrast, **Marker Data** adopts a comprehensive strategy by harnessing the output of the rendered timeline, alongside its associated FCPXML, to generate thumbnails encompassing both stills and GIFs. Additionally, the utilisation of a `.json` format contributes to the creation of an all-encompassing data set.

Comparison matrix between **Marker Data** and **FCPXImageExporter.**

Features   | Marker Data | FCPXImageExporter
:---:   | :---: | :---:
Speed | Fast*  | Fast
Utilises Source Clips | No | Yes
RAW Files| Yes** | No
Effects, Titles & Transitions | Yes** | No
Creates .json Data Set | Yes | No
Creates .csv Data Set | Yes | No
Creates GIFs | Yes | No
Burn-Ins of Labels | Yes | No
Cost | Free & Open Source | Paid

**Dependent on your Mac’s hardware. With Apple Silicon, you can get faster results.*
***Rendered Timeline*

## Does Marker Data replaces Producer's Best Friend?

Contrary to negation, **Producer’s Best Friend** serves as a complement rather than a contradiction. It stands as the optimal application for crafting comprehensive spreadsheet reports compatible with platforms such as Numbers, Excel, Preview, and others. This versatile tool adeptly encompasses diverse elements, including Video Clips, Audio Clips, Titles, Generators, Markers, Keywords, Effects, and Transitions.

In contrast, **Marker Data** specialises solely in the extraction of information pertinent to markers and their associated metadata. It confines its focus to this specific domain, providing a nuanced and refined functionality distinct from the broader spectrum covered by Producer’s Best Friend.

## Can Marker Data's Data Set be used with other applications?

1. Yes.
2. All **Marker Data** files are stored in **Export Destination** folder.
3. In each sub folders, you will find the `*.csv` file with the accompanying images auto named.
4. You can import the `*.csv` to any application that accepts it.

## What constitutes an optimal procedural methodology for the nomenclature of Visual Effects Identification (VFX IDs) within a workflow?

Every project is different. But you can utilise this basic example.

``` VFX ID Example
XYZ701_150_010 - COOPER APPEARS NEAR PLANET SATURN
```

- **XYZ** is a 2-6 character code for the show or movie name
- **701** is a 3 digit episode number. For a standalone movie that is not episodic, any three digit number will suffice
- **150** is the scene number
- **010** is the shot number for the specific VFX shot within the scene
- **COOPER APPEARS NEAR PLANET SATURN** is the descriptive name of the shot

## To what extent does the compatibility of Marker Data with DaVinci Resolve, given its support for FCPXML?

Regrettably, despite the capacity to import and export FCPXMLs within **DaVinci Resolve**, the compatibility of Marker metadata is not integrated into the FCPXML format.

## What rationale underlies the utilisation of Notion v2 Tokens in lieu of official API connections provided by Notion?

The official API provided by Notion currently lacks the capability for direct image uploads and the seamless merging of page icons. Furthermore, it does not offer support for automatic linking or the creation of new entries in relation columns based on their respective values. The prospect of revisiting and updating our internal components will be considered as Notion continues to expand and enhance the functionality of their APIs.

## Is there a contemplation for extending support to additional database platforms in the foreseeable future?

At present, our primary emphasis lies in the steadfast support and enhancement of integration capabilities with Notion and Airtable—two widely acclaimed platforms embraced by users and companies across the global Film and TV industry. The development of robust internal components for both [Notion](https://github.com/TheAcharya/csv2notion-neo) and [Airtable](https://github.com/TheAcharya/Airlift) has demanded a significant investment of time and effort.

Within the expansive landscape of database and productivity solutions, emerging platforms such as [Coda](https://coda.io/), [Baserow](https://baserow.io/), [AppFlowy](https://appflowy.io/), and Microsoft’s [Loop](https://loop.microsoft.com/learn) are gaining prominence.

Should you have specific use cases or preferences for other platforms, we encourage you to initiate a thoughtful [discussion](https://github.com/TheAcharya/MarkerData/discussions). It is essential to note that the incorporation of additional platforms will be contingent upon the availability of compatible API libraries.

## Could Marker Data extract and convert Final Cut Pro's Marker metadata to another format?

Certainly, such an endeavour is within our purview. As we continue to refine and advance our Library, the augmentation of [Profiles](https://github.com/TheAcharya/MarkersExtractor/issues?q=is%3Aissue+is%3Aopen+label%3Aprofiles) is a definite consideration for future enhancements.

## What is Marker Data's Privacy Policy?

**Marker Data** is designed to operate solely on your computer, without any collection of personal information. All processes and data manipulations occur locally, ensuring that your sensitive information remains confidential and secure. However, it's important to note that when you choose to upload data to platforms such as [Notion](https://www.notion.so/security) or [Airtable](https://www.airtable.com/company/trust-and-security), your information is subject to their respective privacy policies. We encourage you to read and familiarise yourself with their security & privacy policies to understand how they handle your data. Rest assured, our commitment to privacy means you can enjoy the benefits of our application without compromising your personal data.

## Is Marker Data free to use?

Yes. But you can [sponsor](https://github.com/sponsors/TheAcharya) us if you find **Marker Data** useful.

