---
label: Image
icon: image
order: -4
---
# Image Settings

![](/assets/md-image-settings.png)

## File Creation

### Naming Mode

Naming Mode allows you to select your preferred `Marker IDs` and image `Filenames` scheme. By [!badge text="Default"] **Marker Data** will use Marker’s `Timecode` as its `Marker ID`. If the project name was `Demo V1`, **Marker Data** would generate the `Marker ID` as `Demo_V1_Timecode` and it will utilise the same `Marker ID` for the image `Filename` as well.

Depending on your workflow, you can also select `Name` or `Notes` as your `Marker ID`. These could be ideal for creating VFX Database. For both `Name` and `Notes`, it is ideal that you input unique text values. If your text values were found to be identical, **Marker Data** would automatically append a numerical suffix at the end of the filename.

![Final Cut Pro's Time Display](/assets/md-image-settings_01.png)

Select your desired Naming Mode.
- **Timecode** [!badge text="Default"]
- **Name**
- **Notes**

### Image Format

By [!badge text="Default"] **Marker Data** will extract and export the images in `PNG` stills. You have the option to select `JPG` or animated `GIF`.

Select your desired Image Format.
- **PNG** [!badge text="Default"]
- **JPG**
- **GIF**

!!!info Info
The file size of the images would be relatively large when selecting **GIF**.
!!!

## Image Size

### Width

By [!badge text="Default"] `Width` selection is disabled. **Marker Data** would automatically use the exact dimensions from your exported video file. When enabled, you can manually limit image width while keeping its aspect ratio.

### Height

By [!badge text="Default"] `Height` selection is disabled. **Marker Data** would automatically use the exact dimensions from your exported video file. When enabled, you can manually limit image height while keeping its aspect ratio.

### Size (%)

By [!badge text="Default"] `Size (%)` is set to `100` for both `PNG` and `JPG`  Image Format. For `GIF` the [!badge text="Default"] value is set to `50`. 

If your original exported video file had dimensions of `1920 x 1080`; when setting `Size (%)` value to `50`, the extracted images would be in `960 x 540`.

!!!info Info
For **GIF** Image Format we do not recommend setting the `Size (%)` value to be more than 60.
!!!

## JPG

### Quality

By [!badge text="Default"] `Quality` is greyed out. It is only available for `JPG` Image Format. The [!badge text="Default"] value is set to `100`.

## GIF

### FPS

### Span (Sec)