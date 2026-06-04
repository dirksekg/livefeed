# EHS Live Feed

This GitHub Pages site displays a YouTube live feed full-screen for building monitors.

Live page:

```text
https://dirksekg.github.io/livefeed/
```

## How To Change The Live Feed

Change the URL used in the carousel app. You do not need to edit GitHub, `index.html`, or a Google Sheet.

Use this format:

```text
https://dirksekg.github.io/livefeed/?v=YOUTUBE_VIDEO_ID
```

Example:

```text
https://dirksekg.github.io/livefeed/?v=v90fGYoHgco
```

## How To Find The YouTube Video ID

The video ID is the 11-character code in the YouTube link.

For this YouTube live URL:

```text
https://www.youtube.com/live/v90fGYoHgco?si=a4wirkC6-sILHlhs
```

The video ID is:

```text
v90fGYoHgco
```

So the carousel URL should be:

```text
https://dirksekg.github.io/livefeed/?v=v90fGYoHgco
```

## Debug Mode

If the feed is not showing correctly, add `&debug=1` to the end of the URL:

```text
https://dirksekg.github.io/livefeed/?v=v90fGYoHgco&debug=1
```

Debug mode shows what video ID the page found and what YouTube embed URL it created.

Remove `&debug=1` before using the URL on public monitors.

## Notes

- The page autoplays muted, which is required for reliable autoplay in Chrome.
- YouTube controls are hidden as much as YouTube allows.
- The page has no title, border, margin, scrollbar, or extra visual elements.
- If the YouTube live feed itself is not active or does not allow embedding, the page may stay black or show a YouTube message.
