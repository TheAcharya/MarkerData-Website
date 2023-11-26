---
icon: key
expanded: true
order: -4
---
# Dropbox Prerequisite

Airtable's API does not allow direct uploading of attachments. In order to upload an attachment via Airtable's API, the attachment must first exist at a publicly accessible url. To mitigate this problem, **Marker Data** has integrated Dropbox into its internal Airtable client. Dropbox’s basic account offers 2GB of free storage. It should be adequate for most operations. Once you upload your attachments to Airtable, you can delete the files from your Dropbox account thereafter.

## Obtain your Dropbox's App key:

1. Login to your [Dropbox's App Console](https://www.dropbox.com/developers/apps){target=“_blank”} account via a web browser.
2. Click on ‘Create app’ button.
3. Choose Scoped access.
4. Choose Full Dropbox access.
5. Give your App a name. _The name of the App can be unique and personal to you._
6. Click on ‘Create app’ button.

![Create a new app on the DBX Platform](/assets/dropbox_01.png)

7. Go to the Permissions tab.
8. Set the permissions as shown on the screenshot.
9. Click on 'Submit' at the bottom.

![Setting the permissions](/assets/dropbox_02.png)

10. Go to the Settings tab.
11. You will see your App key.

![App key](/assets/dropbox_03.png)

12. It is encouraged that you to copy it to your clipboard and store it somewhere safe.
