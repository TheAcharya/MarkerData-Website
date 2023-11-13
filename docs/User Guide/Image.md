---
label: Image
icon: image
order: -4
---
# Image Settings

![Image Settings](/assets/md-image-settings.png)

## File Creation

### Naming Mode

[!badge variant="success" text="Naming Mode"] allows you to select your preferred `Marker IDs` and image `file-name` scheme. By [!badge text="Default"] **Marker Data** will use Marker’s `Timecode` as its `Marker ID`. If the project name was `Demo V1`, **Marker Data** would generate the `Marker ID` as `Demo_V1_Timecode` and it will utilise the same `Marker ID` for the image `file-name` as well.

Depending on your workflow, you can also select `Name` or `Notes` as your `Marker ID`. These would be ideal for creating [VFX Database](/faq.md#what-is-the-appropriate-workflow-for-naming-vfx-ids). For both `Name` and `Notes`, it is recommended that you input unique text values. If your text values were found to be identical, **Marker Data** would automatically append a numerical suffix at the end of the filename.

![Selecting Naming Mode](/assets/md-image-settings_01.png)

Select your desired Naming Mode.
- **Timecode** [!badge text="Default"]
- **Name**
- **Notes**

### Image Format

By [!badge text="Default"] **Marker Data** will extract and export the [!badge variant="success" text="Image Format"] in `PNG` stills. You have the option to select `JPG` or animated `GIF`.

Select your desired Image Format.
- **PNG** [!badge text="Default"]
- **JPG**
- **GIF**

!!!info Info
The file size of the images would be drastically large when selecting `GIF`.
!!!

## Image Size

### Width

[!badge variant="success" text="Width"] selection is disabled by [!badge text="Default"]. **Marker Data** would automatically use the exact dimensions from your exported video file. When enabled, you can manually limit image width while keeping its aspect ratio.

### Height

[!badge variant="success" text="Height"] selection is disabled by [!badge text="Default"]. **Marker Data** would automatically use the exact dimensions from your exported video file. When enabled, you can manually limit image height while keeping its aspect ratio.

### Size (%)

[!badge variant="success" text="Size (%)"] is set to `100` for both `PNG` and `JPG`  [!badge variant="success" text="Image Format"] by [!badge text="Default"]. For `GIF` the [!badge text="Default"] value is set to `50`. 

If your original exported video file had dimensions of `1920 x 1080`; when setting `Size (%)` value to `50`, the extracted images would be in `960 x 540`.

!!!info Info
For `GIF` Image Format we do not recommend setting the [!badge variant="success" text="Size (%)"] value to be more than `60`.
!!!

## JPG

### Quality

By [!badge text="Default"] `Quality` is greyed out. It is only available for `JPG` Image Format. The [!badge text="Default"] value is set to `100`.

![Quality set to 100](/assets/md-image-settings_02.jpg) 

![Quality set to 10](/assets/md-image-settings_03.jpg)

!!!info Info
You can right-click on the above images and save them to your computer to make file-size and compression comparison.
!!!

## GIF

### FPS

[!badge variant="success" text="FPS"] is greyed out by [!badge text="Default"]. It is only available for `GIF` [!badge variant="success" text="Image Format"]. The [!badge text="Default"] value is set to `10`.

### Span (Sec)

[!badge variant="success" text="Size (%)"] is greyed out by [!badge text="Default"]. It is only available for `GIF` [!badge variant="success" text="Image Format"]. The [!badge text="Default"] value is set to `2`.

![GIF with 10 FPS and 2 Sec Span](/assets/md-image-settings_04.gif) 

![GIF with 15 FPS and 3 Sec Span](/assets/md-image-settings_05.gif)

!!!info Info
For `GIF` [!badge variant="success" text="Image Format"] we do not recommend setting the `FPS` value to be more than `15` and setting the [!badge variant="success" text="Size (%)"] value to be more than `3`.
!!!

!!!info Info
You can right-click on the above images and save them to your computer to make file-size comparison.
!!!