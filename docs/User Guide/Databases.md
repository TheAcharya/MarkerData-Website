---
label: Databases
icon: server
order: -8
---
# Database Settings

![Database Settings](/assets/md-database-settings.png)

!!!info Info
Delve deeper into the distinctions and parallels between Notion and Airtable [here](/databases/database-platforms).
!!!

## Creating Notion Database Profile

![Create Notion Profile](/assets/md-database-settings_01.png)

!!!info Info
For Notion Profile, it is strongly advised that users utilise the provided Notion's [Marker Data Template](/user-guide/databases/#notion-template).
!!!

1. Click on the `+` button to Create Database Profile.
2. Enter a Profile Name.
3. For Notion Platform, click on the `Notion` tab.
4. Click `Save` once values are entered.

==- Notion Workspace

Enter your [Notion Workspace Name](/databases/notion-prerequisite#obtain-your-workspace-name) here.

==- Notion V2 Token

Enter your [Notion V2 Token](/databases/notion-prerequisite#obtain-your-session-token) here.

==- Notion Database URL

Enter your [Notion Database URL](/databases/notion-prerequisite##obtain-your-database-url) here. In the absence of a provided Notion Database URL, **Marker Data** will upload all entries of the Marker Metadata from Final Cut Pro into Notion. However, it is strongly advised that you to duplicate the supplied Notion Template by accessing the provided link. Subsequently, you can acquire the link from your duplicated Notion Template within your Workspace.

==- Rename Key Column

By [!badge text="Default"] **Marker Data** will designate the Notion's Key Column with the nomenclature of `Marker ID`. However, you retain the flexibility to establish an alternative form of Notion Database by integrating Marker Metadata from Final Cut Pro. To illustrate, you have the capability to designate your Notion's Key Column as, for instance, `Shot Code`. Upon configuring this setting in Notion, you may then input the same corresponding value in this field as `Shot Code`.

==- Merge Only

Merge Only offers users selectively merge or update individual columns within a Notion Database. By [!badge text="Default"], the column selection feature of Merge Only remains inactive. The utilisation of Merge Only is only possible when Notion Database URL is provided.

!!!info Info
The utilisation of the 'Merge Only' column feature is presently confined exclusive to the Notion Database Profile.
!!!

===

## Creating Airtable Database Profile

![Create Airtable Profile](/assets/md-database-settings_02.png)

!!!info Info
For Airtable Profile, it is imperative to underscore that users are mandated to utilise the provided Airtable's [Marker Data Template](/user-guide/databases/#airtable-template).
!!!

1. Click on the `+` button to Create Database Profile.
2. Enter a Profile Name.
3. For Airtable Platform, click on the `Airtable` tab.
4. Click `Save` once values are entered.

==- Airtable Token

Enter your [Airtable Token](/databases/airtable-prerequisite#obtain-your-workspace-name) here.

==- Airtable Base ID

 Enter your [Airtable Base ID](/databases/airtable-prerequisite#obtain-your-base-id--table-id) here.
 
==- Airtable Table ID

Enter your [Airtable Table ID](/databases/airtable-prerequisite#obtain-your-base-id--table-id) here.

==- Rename Key Column

By [!badge text="Default"] **Marker Data** will designate the Airtable's Key Column with the nomenclature of `Marker ID`. However, you retain the flexibility to establish an alternative form of Airtable Database by integrating Marker Metadata from Final Cut Pro. To illustrate, you have the capability to designate your Airtable's Key Column as, for instance, `Shot Code`. Upon configuring this setting in Notion, you may then input the same corresponding value in this field as `Shot Code`.

==- Dropbox App Key

Enter your [Dropbox App Key](/databases/dropbox-prerequisite) here. Setting up Dropbox integration is a one-time process. Whenever you duplicate or create a new Airtable Database Profile, the **Marker Data** feature will automatically utilise the pre-existing Dropbox App Key. If there arises a necessity to modify or refresh your Dropbox App Key, simply input the new value into the Dropbox App Key field and proceed accordingly.

![Dropbox Setup](/assets/md-database-settings_dropbox.gif)

!!!info Info
It is advisable to ensure prior login to your Dropbox Account has been completed.
!!!

1. Ensure that all prescribed steps [delineated here](/databases/dropbox-prerequisite) have been completed.
2. Copy your App Key.
3. Paste it in the `Dropbox App Key` field.
4. Press `Continue`.
5. **Marker Data** will launch Terminal.
6. Highlight the full URL, right-click to `Open Link`.
7. Your default browser will be launched with the URL.
8. Click `Continue` and click `Allow`.
9. Copy your unique `Authorisation code`.
10. Return back to the Terminal session, and paste the `Authorisation code`.
11. Press `Enter` on your keyboard.
12. Once `Done` appears on the Terminal session, you can close your Terminal window.
13. You will see `Dropbox configured` text on your Airtable Database Profile window.

!!!info Info
Upon initial utilisation, **Marker Data** will create a directory titled `Marker Data` within the root of your Dropbox and proceed to upload accordingly.
!!!

===

## Duplicate Database Profile

You have the ability to duplicate any Database Profile by clicking on the `Duplicate` button.

!!!info Info
Through the utilisation of the `Duplicate` button, you can effortlessly generate numerous Database Profiles. The sole prerequisite is the substitution of the Database URL for Notion or the Base ID and Table ID for Airtable, thereby facilitating the quick replication of Database Profiles.
!!!

## Edit Database Profile

You have the ability to edit any Database Profile by clicking on the `Edit` button.

!!!info Info
Upon the expiration of values, such as the `Token`, upon obtaining a renewed set of Tokens, you can update your pre-existing Database Profiles. This task is accomplished by clicking the `Edit` button, followed by `Save` button.
!!!

## Delete Database Profile

1. Click on the `-` button.
2. You will be prompted for confirmation before deletion.

## Open Database Folder in Finder

Select the `Open Database Folder in Finder` link to unveil the Finder directory housing the Database Profile files. You can copy the `.json` files to another location for the purpose of creating backups and restoration of your Database Profile files.

## Notion Template

| Preview | Template Link |
|---|---|
| Image | [!button variant="primary" target="blank" icon="link-external" text="Marker Data Template"](https://theacharya.co/) |
| Image | [!button variant="primary" target="blank" icon="link-external" text="Frame Library Template"](https://theacharya.co/) |

[!button icon="<svg width="100" height="100" viewBox="0 0 100 100" fill="none" xmlns="http://www.w3.org/2000/svg">
  <path d="M6.017 4.313l55.333 -4.087c6.797 -0.583 8.543 -0.19 12.817 2.917l17.663 12.443c2.913 2.14 3.883 2.723 3.883 5.053v68.243c0 4.277 -1.553 6.807 -6.99 7.193L24.467 99.967c-4.08 0.193 -6.023 -0.39 -8.16 -3.113L3.3 79.94c-2.333 -3.113 -3.3 -5.443 -3.3 -8.167V11.113c0 -3.497 1.553 -6.413 6.017 -6.8z" fill="#fff"/>
  <path fill-rule="evenodd" clip-rule="evenodd" d="M61.35 0.227l-55.333 4.087C1.553 4.7 0 7.617 0 11.113v60.66c0 2.723 0.967 5.053 3.3 8.167l13.007 16.913c2.137 2.723 4.08 3.307 8.16 3.113l64.257 -3.89c5.433 -0.387 6.99 -2.917 6.99 -7.193V20.64c0 -2.21 -0.873 -2.847 -3.443 -4.733L74.167 3.143c-4.273 -3.107 -6.02 -3.5 -12.817 -2.917zM25.92 19.523c-5.247 0.353 -6.437 0.433 -9.417 -1.99L8.927 11.507c-0.77 -0.78 -0.383 -1.753 1.557 -1.947l53.193 -3.887c4.467 -0.39 6.793 1.167 8.54 2.527l9.123 6.61c0.39 0.197 1.36 1.36 0.193 1.36l-54.933 3.307 -0.68 0.047zM19.803 88.3V30.367c0 -2.53 0.777 -3.697 3.103 -3.893L86 22.78c2.14 -0.193 3.107 1.167 3.107 3.693v57.547c0 2.53 -0.39 4.67 -3.883 4.863l-60.377 3.5c-3.493 0.193 -5.043 -0.97 -5.043 -4.083zm59.6 -54.827c0.387 1.75 0 3.5 -1.75 3.7l-2.91 0.577v42.773c-2.527 1.36 -4.853 2.137 -6.797 2.137 -3.107 0 -3.883 -0.973 -6.21 -3.887l-19.03 -29.94v28.967l6.02 1.363s0 3.5 -4.857 3.5l-13.39 0.777c-0.39 -0.78 0 -2.723 1.357 -3.11l3.497 -0.97v-38.3L30.48 40.667c-0.39 -1.75 0.58 -4.277 3.3 -4.473l14.367 -0.967 19.8 30.327v-26.83l-5.047 -0.58c-0.39 -2.143 1.163 -3.7 3.103 -3.89l13.4 -0.78z" fill="#000"/>
</svg>" text="Marker Data Template"](https://theacharya.co/)

## Airtable Template

| Preview | Template Link |
|---|---|
| Image | [!button variant="primary" target="blank" icon="link-external" text="Marker Data Template"](https://theacharya.co/) |