---
label: Databases
icon: server
order: -8
---
# Database Settings

!!!info Info
Learn more about the differences and similarities between Notion and Airtable [here](/databases/database-platforms).
!!!

![Database Settings](/assets/md-database-settings.png)

## Creating Notion Database Profile

![Create Notion Profile](/assets/md-database-settings_01.png)

1. Click on the `+` button to Create Database Profile.
2. Enter a Profile Name.
3. For Notion Platform, click on the `Notion` tab.
4. Click `Save` once values are entered.

=== Notion Workspace
Enter your [Notion Workspace Name](/databases/notion-prerequisite#obtain-your-workspace-name) here.
=== Notion V2 Token
 Enter your [Notion V2 Token](/databases/notion-prerequisite#obtain-your-session-token) here.
=== Notion Database URL
Enter your [Notion Database URL](/databases/notion-prerequisite##obtain-your-database-url) here. In the absence of a provided Notion Database URL, **Marker Data** will upload all entries of the Marker Metadata from Final Cut Pro into Notion. However, it is strongly advised that you to duplicate the supplied Notion Template by accessing the provided link. Subsequently, you can acquire the link from your duplicated Notion Template within your Workspace.
=== Rename Key Column
By [!badge text="Default"] **Marker Data** will designate the Notion's Key Column with the nomenclature of `Marker ID`. However, you retain the flexibility to establish an alternative form of Notion Database by integrating Marker Metadata from Final Cut Pro. To illustrate, you have the capability to designate your Notion's Key Column as, for instance, `Shot Code`. Upon configuring this setting in Notion, you may then input the same corresponding value in this field as `Shot Code`.
=== Merge Only
Merge Only offers users selectively merge or update individual columns within a Notion Database. By [!badge text="Default"], the column selection feature of Merge Only remains inactive. The utilisation of Merge Only is only possible when Notion Database URL is provided.
===

## Creating Airtable Database Profile

![Create Airtable Profile](/assets/md-database-settings_02.png)

1. Click on the `+` button to Create Database Profile.
2. Enter a Profile Name.
3. For Airtable Platform, click on the `Airtable` tab.
4. Click `Save` once values are entered.

=== Airtable Token
Enter your [Airtable Token](/databases/airtable-prerequisite#obtain-your-workspace-name) here.
=== Airtable Base ID
 Enter your [Airtable Base ID](/databases/airtable-prerequisite#obtain-your-base-id--table-id) here.
=== Airtable Table ID
Enter your [Airtable Table ID](/databases/airtable-prerequisite#obtain-your-base-id--table-id) here.
=== Rename Key Column
By [!badge text="Default"] **Marker Data** will designate the Airtable's Key Column with the nomenclature of `Marker ID`. However, you retain the flexibility to establish an alternative form of Airtable Database by integrating Marker Metadata from Final Cut Pro. To illustrate, you have the capability to designate your Airtable's Key Column as, for instance, `Shot Code`. Upon configuring this setting in Notion, you may then input the same corresponding value in this field as `Shot Code`.
=== Dropbox App Key
Enter your [Dropbox App Key](/databases/dropbox-prerequisite) here.
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