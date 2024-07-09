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

## Marker Data shows Failed to upload completely.

![Failed to upload completely](/assets/md-failed-to-upload-completely.png)

When **Marker Data** displays a `Failed to upload completely` error, it may be due to couple of factors. One potential cause is that you are using an Intel-based Mac, which is not supported by **Marker Data**. For further information, please refer to this [FAQ](/faq/#does-marker-data-support-intel-based-macs).

If you are utilising a firewall application such as Little Snitch, please ensure that outgoing connections to **Marker Data** are permitted.