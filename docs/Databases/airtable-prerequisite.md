---
icon: key
expanded: true
order: -3
---
# Airtable Prerequisite

## Obtain your Airtable's Personal Access Token:

1. Login to your [Airtable](https://airtable.com/login){target=“_blank”} account via a web browser.
2. Go to [Personal access token](https://airtable.com/create/tokens){target=“_blank”}, click the **Create new token** button to create a new personal access token.
3. Give your token a unique name. This name will be visible in record revision history.
4. Add the following scopes to grant to your token. This controls what API endpoints the token will be able to use.

![Scopes](/assets/airtable_scopes.png)

5. Click **add a base** to grant the token access to a base or workspace.
!!!info Info
You can grant access to any combination and number of bases and workspaces. You can also grant access to all workspaces and bases under your account. Keep in mind that the token will only be able to read and write data within the bases and workspaces that have been assigned to it.
!!!

6. Once your token is created, the token will only be shown to you once, it is encouraged that you to copy it to your clipboard and store it somewhere safe. While you will be able to manage it in [Personal access token](https://airtable.com/create/tokens){target=“_blank”}, the sensitive token itself is not stored for security purposes.

## Obtain your Airtable's Base ID & Table ID:

1. When you have a base open in a compatible web browser, you should see a URL in the address bar that looks similar to the example below:

![Airtable URL](/assets/airtable_url.jpg)

In between each backslash, you will find a string that identifies the base, table, and view IDs.

- Base IDs begin with "app"
- Table IDs begin with "tbl"
- View IDs begin with "viw"

![Airtable URL Reference](/assets/airtable_url_reference.png)

!!!info Info
We only require **Base ID** and **Table ID** for Marker Data
!!!

To read more about attachments and obtaining your Dropbox's App key, please read [Dropbox Prerequisite](/Databases/dropbox-prerequisite.md).