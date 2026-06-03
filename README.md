# Live Feed Display

This is a GitHub Pages display page that fills the whole screen with a YouTube live feed.

The page reads the current YouTube URL from a published Google Sheet once per minute.
It only updates the iframe when the `Version` value changes.

## Google Sheet setup

Create a Google Sheet with a tab named:

Settings

Use this format:

| Setting | Value |
|---|---|
| YouTubeURL | https://www.youtube.com/watch?v=IVmL3diwJuw |
| Version | 1 |

When staff need to change the feed:
1. Paste the new YouTube URL in the YouTubeURL value cell.
2. Increase the Version number by 1.

Example:
Version 1 becomes Version 2.

## Publish the Google Sheet

In Google Sheets:
1. File
2. Share
3. Publish to web
4. Choose the Settings sheet
5. Publish

## Update index.html

Open index.html and replace:

PASTE_YOUR_GOOGLE_SHEET_ID_HERE

with the Sheet ID from your Google Sheet URL.

Example Google Sheet URL:

https://docs.google.com/spreadsheets/d/1AbCdEfGhIjKlMnOpQrStUvWxYz/edit

The Sheet ID is:

1AbCdEfGhIjKlMnOpQrStUvWxYz

## GitHub Pages setup

Upload index.html to your GitHub repo.

Then:
1. Repo Settings
2. Pages
3. Deploy from branch
4. Branch: main
5. Folder: root
6. Save

Open the GitHub Pages URL in Chrome and enter full screen.
