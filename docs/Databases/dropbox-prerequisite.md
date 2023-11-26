---
icon: key
expanded: true
order: -4
---
# Dropbox Prerequisite

Airtable's API does not allow direct uploading of attachments. In order to upload an attachment via Airtable's API, the attachment must first exist at a publicly accessible url. To mitigate this problem, **Marker Data** has integrated Dropbox into its internal Airtable client. Dropbox’s basic account offers 2GB of free storage. We believe it would be adequate for most operations Once your attachments are uploaded by Airtable, you can delete the files from your Dropbox account.

## Obtain your Airtable's Personal Access Token:


1. Right-click and save [dropbox-token.json](https://raw.githubusercontent.com/TheAcharya/Airlift/main/assets/dropbox-token.json) file to your computer.
2. When using `--dropbox-token` make sure you input the full `PATH` of `dropbox-token.json` file.
3. Login to your [Dropbox's App Console](https://www.dropbox.com/developers/apps) account via a web browser.
4. Click on ‘Create app’ button.
5. Choose Scoped access.
6. Choose Full Dropbox access.
7. Give your App a name. _The name of the App can be unique and personal to you._
8. Click on ‘Create app’ button.

<p align="center"> <img src="https://github.com/TheAcharya/Airlift/blob/main/assets/dropbox_01.png?raw=true"> </p>

7. Go to the Permissions tab.
8. Set the permissions as shown on the screenshot.
9. Click on 'Submit' at the bottom.

<p align="center"> <img src="https://github.com/TheAcharya/Airlift/blob/main/assets/dropbox_02.png?raw=true"> </p>

10. Go to the Settings tab.
11. Copy your App key and paste into your `dropbox-token.json` file. Where `REPLACE` is your App key.

<p align="center"> <img src="https://github.com/TheAcharya/Airlift/blob/main/assets/dropbox_03.png?raw=true"> </p>

```json
{
  "app_key": "REPLACE"
}
```

12. On first usage of Airlift, you will be promted to visit Dropbox.
13. Copy and paste the full Dropbox URL into your browser.

```txt
INFO: Validation done!
INFO: All the columns are verified and present in both the file and Airtable!
1. Go to: https://www.dropbox.com/oauth2/authorize?response_type=code&client_id=6zh18qgnw37ifpp&token_access_type=offline&code_challenge=TphrwcwmRtkGawgxFvWQcROFMbjsTeba9BGv0Lgi0nw&code_challenge_method=S256
2. Click "Allow" (you might have to log in first).
3. Copy the authorization code.
Enter the authorization code here:    
```

<p align="center"> <img src="https://github.com/TheAcharya/Airlift/blob/main/assets/dropbox_04.png?raw=true"> </p>

14. Click Continue.

<p align="center"> <img src="https://github.com/TheAcharya/Airlift/blob/main/assets/dropbox_04.png?raw=true"> </p>

15. Click Allow.

<p align="center"> <img src="https://github.com/TheAcharya/Airlift/blob/main/assets/dropbox_05.png?raw=true"> </p>

16. You will be presented with your authorization code. Copy your authorization code.

<p align="center"> <img src="https://github.com/TheAcharya/Airlift/blob/main/assets/dropbox_06.png?raw=true"> </p>

```bash
Enter the authorization code here:    XXXZZaa0-poAAAAAAABZNgc9CwNdyryqoRAi4fxP2aU
```

17. Paste it back into the terminal.
18. Airlift would update and store your Dropbox refresh token into your `dropbox-token.json` file.
19. This is a one time procress. You will not be asked again.

**Do not share your access json token file with anyone.**