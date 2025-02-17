---
label: Troubleshooting
icon: tools
order: -95
---
# Troubleshooting

Below, you will find a comprehensive list of common issues users may encounter, accompanied by solutions to resolve them.

## How to access the logs in Marker Data?

To access the logs for **Marker Data**, navigate to the `Help` menu and select `Open Logs`.

## Marker Data's Workflow Extension is not functioning. 

To ensure optimal functionality of **Marker Data**, please ensure it is installed within the Applications folder.

## Why is the upload speed to Notion slow?

The slow upload speed to Notion could be attributed to potential issues with Notion's servers or regional server connectivity. Please verify the current [status](https://status.notion.so/) of Notion's servers.

## Why are there no images in the extract folder?

Please ensure that you are using **Marker Data**'s [Share Destination](/user-guide/share-destination). Images will not be extracted when using **Marker Data**'s [Workflow Extension](/user-guide/workflow-extension).

## Marker Data shows Failed to complete upload.

![Failed to complete upload](/assets/md-failed-to-complete-upload.png)

When **Marker Data** displays a `Failed to complete upload` error, it may be attributed to various underlying causes. If you are utilising a firewall application such as Little Snitch, please ensure that outgoing connections to **Marker Data** are permitted.

### Notion

If you encounter issues uploading to your Notion Database, please follow these steps to troubleshoot:

1. Navigate to the `Help` menu and select `Open Logs`.
2. Open the log file `csv2notion-neo_log.txt`.
3. Scroll down to review the most recent entries.

If you observe the error messages `HTTPError: 401 Client Error: Unauthorized for url` or `Invalid Notion token`, it is likely that either your Notion Database URL is incorrect or your Notion v2 Token has expired. For detailed instructions on resolving these issues, please refer to the [Notion Prerequisite](/databases/notion-prerequisite) documentation.

### Airtable

If you encounter issues uploading to your Airtable Database, please follow these steps to troubleshoot:

1. Navigate to the `Help` menu and select `Open Logs`.
2. Open the log file `airlift_log.txt`.
3. Scroll down to review the most recent entries.

If you observe the error messages `Authentication required` or `Invalid permissions, or the requested model was not found.`, it is likely that either your Airtable Token is incorrect or your Airtable Base ID & Table ID is incorrect. For detailed instructions on resolving these issues, please refer to the [Airtable Prerequisite](/databases/airtable-prerequisite) documentation.

If you observe the error message `Error in call to API function "files/create_folder": Your app is not permitted to access this endpoint because it does not have the required scope \'files.content.write\'. The owner of the app can enable the scope for the app using the Permissions tab on the App Console.')`, it is likely that the required scopes for the app utilising the Permissions tab within the Dropbox's App Console is not checked. For detailed instructions on resolving these issues, please refer to the [Dropbox Prerequisite](/databases/dropbox-prerequisite) documentation. After you have checked your and submitted the scopes, you must to re-create and start over your Dropbox refresh token again. For detailed instructions on resolving these issues, please refer to the [Creating Airtable Database Profile](/user-guide/databases/#creating-airtable-database-profile) documentation.

## Marker Data shows Failed to upload completely.

![Failed to upload completely](/assets/md-failed-to-upload-completely.png)

When **Marker Data** displays a `Failed to upload completely` error, it may be due to couple of factors. One potential cause is that you are using an Intel-based Mac, which is not supported by **Marker Data**. Starting with **Marker Data** version 1.1.0, application is exclusively build and optimised for Apple Silicon only. For further information, please refer to this [FAQ](/faq/#does-marker-data-support-intel-based-macs).

If you are utilising a firewall application such as Little Snitch, please ensure that outgoing connections to **Marker Data** are permitted.

## I have verified and ensured that all Notion prerequisites are met and entered correctly. However, Marker Data still shows Failed to upload completely.

1. Navigate to the `Help` menu and select `Open Logs`.
2. Open the log file `csv2notion-neo_log.txt`.
3. Scroll down to review the most recent entries.

If you encounter error messages similar to the one displayed, it may indicate that Notion has updated its APIs, requiring an update to Marker Data's Notion module.

```bash
2025-02-15 10:23:02,118 [ERROR   ] Error at division
Traceback (most recent call last):
  File "csv2notion_neo/cli.py", line 58, in cli
  File "csv2notion_neo/cli_steps.py", line 80, in upload_rows
  File "tqdm/std.py", line 1181, in __iter__
  File "csv2notion_neo/utils_threading.py", line 39, in process_iter
  File "csv2notion_neo/utils_threading.py", line 39, in <genexpr>
  File "concurrent/futures/_base.py", line 437, in result
  File "concurrent/futures/_base.py", line 389, in __get_result
  File "concurrent/futures/thread.py", line 57, in run
  File "csv2notion_neo/utils_threading.py", line 27, in worker
  File "csv2notion_neo/notion_uploader.py", line 33, in upload_row
  File "csv2notion_neo/notion_uploader.py", line 50, in _get_db_row
  File "csv2notion_neo/notion_db.py", line 106, in add_row
  File "csv2notion_neo/notion_db_collection.py", line 39, in add_row_block
  File "csv2notion_neo/notion_db_collection.py", line 69, in _add_row_block
  File "csv2notion_neo/notion_row.py", line 46, in icon
  File "csv2notion_neo/notion_row_upload_file.py", line 21, in upload_filetype
  File "csv2notion_neo/notion_row_upload_file.py", line 41, in upload_file
```

Occasionally, **Marker Data**'s Notion module would become non-functional when Notion updates its APIs. This occurs due to the reliance on [unofficial APIs](/faq/#what-rationale-underlies-the-utilisation-of-notion-v2-tokens-in-lieu-of-official-api-provided-by-notion).

If you encounter such an problem, please open an [issue](https://github.com/TheAcharya/MarkerData/issues). With time and thorough investigation, we will release an update for **Marker Data**. However, the update may not be immediate, as it depends on our availability to analyse and resolve the issue. We appreciate your patience and understanding.

## Module Status

To streamline our internal testing process, we have implemented an automated weekly validation of Marker Data’s module.

Tests   | Status | Schedule
---    | --- | ---
Notion  | [![notion_image_upload_test](https://github.com/TheAcharya/csv2notion-neo/actions/workflows/notion_image_upload_test.yml/badge.svg)](https://github.com/TheAcharya/csv2notion-neo/actions/workflows/notion_image_upload_test.yml) | Scheduled weekly on Saturdays at 8:00 AM Singapore time

If the badge is green, indicating a successful test, it confirms that our modules are compatible with the supported database platforms. However, if the badge turns red, signalling a failure, an update may be necessary to ensure continued compatibility.

