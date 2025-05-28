---
icon: key
expanded: true
order: -2
---
# Notion Prerequisite

!!!warning Warning
Notion applies variable rate limits to its API. On average, it supports approximately three requests per second. While occasional bursts exceeding this average may be permitted, they are not guaranteed and should not be relied upon. Additionally, Notion's rate limits are subject to change at any time, and we have no control over such modifications.

To prevent errors such as `HTTP 500 (Internal Server Error)` or `HTTP 429 (Too Many Requests)`, users are strongly advised not to upload large Data Set (e.g., 99 images) in a single batch. Instead, it is recommended to upload data in smaller batches of no more than 50 items at a time, with a short pause between batches to avoid triggering rate limits.

For the most current information on Notion’s rate limiting policies, please refer to their [official documentation](https://developers.notion.com/reference/request-limits).
!!!

## Obtain your Workspace Name

![Workspace Name](/assets/notion_workspace.png)

1. To see your Workspace Name go to `Settings & members` at the top of the left sidebar. In the window that pops up, click on the `Settings` tab.
2. If your Workspace name is `Acme Inc.`, you are required to copy the entire value `Acme Inc.` as such.

## Obtain your Session Token

1. Login to your [Notion](https://www.notion.so/login) account via a web browser.
2. Find and copy the entire `token_v2` value including `v03%3` from your Notion session.

!!!info Info
Your Notion v2 Token should start with `v03%3...`
!!!

==- Safari
Enable Web Inspector

- If you don’t see the Develop menu in the menu bar, choose Safari, Settings, click Advanced, then select “Show features for web developers”.
- Press `⌥ + ⌘ + i` to show Web Inspector.

<video controls width="1920">
  <source src="/assets/safari.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
===

==- Brave, Chrome, Edge or Arc
1. Press `⌥ + ⌘ + i` to show Developer Tools.
2. Go to `Application` tab.
3. Copy and obtain your `token_v2` value.

![Brave's Developer Tools](/assets/brave.png)

===

!!!info Info
Please take note that your Notion v2 Token may expire after some period of time. You would have to obtain it again.
!!!

!!!warning Warning
Do not share your Notion v2 Token with anyone.
!!!

## Obtain your Database URL

1. Go to your Notion Database, and right-click on the view and click **Copy link to view**.

![Copy Notion URL](/assets/notion_url.png)