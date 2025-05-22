---
label: Generating Markers
icon: video
order: -7
---
# Generating Markers

![](/assets/content-banner-marker-toolbox.png)

Users interested in procedural Marker extraction can take advantage of the [Marker Toolbox](https://markertoolbox.io), which offers capabilities for inserting and manipulating Markers. When combined with **Marker Data** and modern chat-based models, this setup enables a cohesive, end-to-end workflow for both programmatic generation and extraction of Markers. Although a generative approach to Marker extraction was initially [explored](https://github.com/TheAcharya/MarkersExtractor/issues/108), it was ultimately considered too specialised for inclusion in **Marker Data**'s roadmap.

## CSV Profile

1. Create Your CSV Profile.

!!!info Info
You can also use TSV, Excel, Notion or Airtable Profile.
!!!

## Configuration Setup

![Configuration Setup](/assets/md-marker-generation-01.gif)

1. [Create Your Configuration](/user-guide/configurations/#add-configuration).
2. You can select your desired Export Destination by clicking on the [Folder Icon](/user-guide/general/#export-destination).
3. You can select `CSV` as your [Extraction Profile](/user-guide/general/#extraction-profile).
4. You can set [Image Format](/user-guide/image/#image-format) to `PNG`.
5. Enable [Swatch](/user-guide/image/#swatch) (Optional).
6. Select your desired [Overlays](/user-guide/label/#overlays) (Optional).
7. Return back to Configurations to [Update Active Configuration](/user-guide/configurations/#update-active-configuration)

## Count Mode

Below is a refined AI prompt template for use with Count Mode. You may input it into your preferred language model, such as [ChatGPT](https://chatgpt.com/), [Claude](https://claude.ai/), or [DeepSeek](https://www.deepseek.com/en). Please ensure that the `Timeline Duration` and `Timeline FPS` values match your timeline’s total duration and frame rate. You may also customise the `Marker Prefix`, `Marker Name Zero Padding`, and `Count` values according to your specific requirements.

### AI Prompt Template

```text
Timeline Duration: “00:02:15:00”
Timeline FPS: “25p”
Marker Prefix: “Marker”
Marker Name Zero Padding: “4”
NLE: “Final Cut Pro”
Mode: “Count”
Count: “10”

Sample List Style
00:00:01:00 - Marker-0001
00:00:02:00 - Marker-0002

Instruction:
Generate a list of marker positions based on the specified “Timeline Duration” and “Timeline FPS”. 
The markers must be evenly spaced and calculated with high precision. 
They should fall strictly within the bounds of the timeline; excluding both the start “00:00:00:00” and the end “Timeline Duration”.

List them in code block.
```

!!!info Info
DeekSeek is used for this demonstration.
!!!

![Count Mode Prompt in DeepSeek](/assets/md-marker-generation-02.gif)

<br>

<video controls width="1920">
  <source src="/assets/md-marker-generation-04.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<br>

1. Click the `Extensions` button on the left side of **Final Cut Pro**’s toolbar.
2. Select `Marker Toolbox` from the `Extensions` menu.
3. Click `Settings` and ensure that your frame rate matches the timeline frame rate in **Final Cut Pro**.
4. Ensure you have clicked `Copied` from DeepSeek’s code block.
5. In `Marker Toolbox`, click `Paste`, then click `Process Comments Locally`. Adjust any Marker's timecode if needed.
6. Click the `Green` button to drag and drop the `Compound Clip` into your timeline.
7. Make sure the `Compound Clip` is aligned with the start of the timeline.
8. From **Final Cut Pro**’s Share menu, select either `Marker Data Source` or `Marker Data H.264`
9. **Marker Data** will start to perform its task.
10. Once the export is complete, save the file to your desired location.

!!!info Info
You can use this same technique for the [Notion Database Profile](/user-guide/databases/#creating-notion-database-profile), the [Airtable Database Profile](/user-guide/databases/#creating-airtable-database-profile) or even when working with [Pagemaker](/user-guide/pagemaker/).
!!!

<hr>

## Interval Mode

Below is a refined AI prompt template for use with Interval Mode. You may input it into your preferred language model, such as [ChatGPT](https://chatgpt.com/), [Claude](https://claude.ai/), or [DeepSeek](https://www.deepseek.com/en). Please ensure that the `Timeline Duration` and `Timeline FPS` values match your timeline’s total duration and frame rate. You may also customise the `Marker Prefix`, `Marker Name Zero Padding`, and `Interval` values according to your specific requirements.

### AI Prompt Template

```text
Timeline Duration: “00:02:30:00”
Timeline FPS: “25p”
Marker Prefix: “Marker”
Marker Name Zero Padding: “4”
NLE: “Final Cut Pro”
Mode: “Interval”
Interval: “70 Frames”

Sample List Style
00:00:01:00 - Marker-0001
00:00:02:00 - Marker-0002

Instruction:
Generate a list of marker positions based on the specified “Timeline Duration” and “Timeline FPS”. 
Markers should be placed at every defined “Interval” within the “Timeline Duration”. 
All calculations must be performed with high precision and accuracy. Marker positions must fall strictly within the bounds of the timeline duration.

List them in code block.
```

!!!info Info
DeekSeek is used for this demonstration.
!!!

![Interval Mode Prompt in DeepSeek](/assets/md-marker-generation-03.gif)

<br>

<video controls width="1920">
  <source src="/assets/md-marker-generation-05.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>

<br>

1. Click the `Extensions` button on the left side of **Final Cut Pro**’s toolbar.
2. Select `Marker Toolbox` from the `Extensions` menu.
3. Click `Settings` and ensure that your frame rate matches the timeline frame rate in **Final Cut Pro**.
4. Ensure you have clicked `Copied` from DeepSeek’s code block.
5. In `Marker Toolbox`, click `Paste`, then click `Process Comments Locally`. Adjust any Marker's timecode if needed.
6. Click the `Green` button to drag and drop the `Compound Clip` into your timeline.
7. Make sure the `Compound Clip` is aligned with the start of the timeline.
8. From **Final Cut Pro**’s Share menu, select either `Marker Data Source` or `Marker Data H.264`
9. **Marker Data** will start to perform its task.
10. Once the export is complete, save the file to your desired location.

!!!info Info
You can use this same technique for the [Notion Database Profile](/user-guide/databases/#creating-notion-database-profile), the [Airtable Database Profile](/user-guide/databases/#creating-airtable-database-profile) or even when working with [Pagemaker](/user-guide/pagemaker/).
!!!

## Afterthoughts

The procedural workflow for Marker extraction and generation opens up a range of compelling use cases. One notable example is the archival of timelines—such as those found in video editing, animation, or narrative design workflows—where users may wish to capture still frames or key moments along the timeline. These snapshots can then be compiled into structured documents using [Pagemaker](/user-guide/pagemaker/), enabling the creation of rich, navigable PDFs that serve as comprehensive visual records.

What makes this workflow particularly powerful is its compatibility with large language models (LLMs). By integrating chat-based models into the pipeline, users can generate sophisticated Marker placement patterns automatically.
