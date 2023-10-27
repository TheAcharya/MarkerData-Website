---
icon: key
expanded: true
order: -3
---
# Airtable Prerequisite

## To obtain your Airtable's Personal Access Token (PATs):

1. Login to your [Airtable](https://airtable.com/login){target=“_blank”} account via a web browser.
2. Go to [Personal access token](https://airtable.com/create/tokens){target=“_blank”}, click the **Create new token** button to create a new personal access token.
3. Give your token a unique name. This name will be visible in record revision history.
4. Add the following scopes to grant to your token. This controls what API endpoints the token will be able to use.

![Scopes](/assets/airtable_scopes.png)

5. Click ‘add a base’ to grant the token access to a base or workspace.
!!!info Info
You can grant access to any combination and number of bases and workspaces. You can also grant access to all workspaces and bases under your account. Keep in mind that the token will only be able to read and write data within the bases and workspaces that have been assigned to it.
!!!

6. Once your token is created, we will only show it to you once, it is encouraged that you to copy it to your clipboard and store it somewhere safe. While you will be able to manage it in [Personal access token](https://airtable.com/create/tokens){target=“_blank”}, the sensitive token itself is not stored for security purposes.