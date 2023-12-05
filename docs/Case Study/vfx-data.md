---
label: VFX Data
icon: pin
order: -1
---
# VFX Data Tracking and Management

[Josh Beal](https://twitter.com/jbkilty){target=“_blank”} makes an excellent comparison of VFX Data Tracking & Management workflow between **Media Composer** and **Final Cut Pro**. Without a doubt, Final Cut Pro’s approach is much superior because of FCPXML’s metadata. **Can we improve the user’s workflow even further?**

[!embed](https://www.youtube.com/watch?v=Md-hNTzr5UE)

## Glaring Pain Points

### Batch exporting still frames for thumbnails & frame identification

You can export still frames from Final Cut Pro. You can add the native **Save Current Frame** preset [destination](https://support.apple.com/en-sg/guide/final-cut-pro/ver9fd008a21/mac){target=“_blank”} to your share menu. Even though you can Batch Export Clips natively, for still frames, you could only do it one by one. However, you can create a [Custom Compressor Setting](https://support.apple.com/en-sg/guide/compressor/cpsr52823a16/mac){target=“_blank”} specifically for batch exporting, still frames. Despite having a **Custom Compressor Setting** you would still need to manually copy and paste those desired clips to compound clips and mark your desired frame.

![Excerpts from Josh Beal’s Video](assets/jb-batch_export_still_frames.gif)

!!!info Info
It just requires too many steps in my textbook. What happens when you have 500 VFX shots?
!!!

### Extracting Marker information & match still’s filename

There is an application called [Producer’s Best Friend](https://intelligentassistance.com/producer-s-best-friend.html){target=“_blank”}. Using Final Cut Pro’s FCPXML file, users can extract all metadata information to a spreadsheet pertaining to any timeline. It is an outstanding tool for generating and extracting specific reports from any Final Cut Pro project.

![Excerpts from Josh Beal’s Video](assets/jb-extract_metadata.gif)

!!!info Info
Again, additional application and further steps are required to created a proper Data Set that has relationship with thumbnails.
!!!

### Sending & Managing VFX Data Set to a Database Application

Josh Beal utilises Airtable to manage his Data Set. Airtable is undoubtedly a powerful cloud-base database application. It has a lot of features when comes to automations, scripting, extensions, report generation and collaboration. But users have to bear a [high cost](https://www.airtable.com/pricing){target=“_blank”} when factoring in collaborative expansion and additional user licenses. Furthermore, additional database views and features are locked behind a higher paywall tier. Having alternative database platforms would be ideal to the end user.

![Excerpts from Josh Beal’s Video](assets/jb-airtable_database.gif)

!!!info Info
The above example shows merging of image’s data set and `.csv`’s data set via Airtable’s [CSV Import Extension](https://support.airtable.com/docs/csv-import-extension){target=“_blank”}. There is still a little manual work involved when mapping data to the appropriate fields.
!!!

### Creating Burn-In labels

There are several ways to create Burn-In labels for your still frames. Josh Beal uses a Final Cut Pro [Effect Template](https://support.apple.com/en-sg/guide/motion/motn141bbb1f/mac){target=“_blank”} created from Apple Motion to create the desired burn-In label for your frames.

![Excerpts from Josh Beal’s Video](assets/jb-burn-ins.gif)

!!!info Info
Using an Effect Template created from Apple Motion is a great approach. It all depends on what are you trying to achieve. Having that custom Effect Template for burn-In labels will always come in handy! What if it can be automated?
!!!