# M3U TV Playlist

A simple static M3U playlist that can be used with IPTV players, media apps, streaming devices, home media systems, smart home dashboards, media servers, and any application that supports loading an M3U playlist from a URL.

## Direct Playlist URL

Copy and paste this URL into any application that supports M3U playlist loading by URL:

```text
https://raw.githubusercontent.com/il90il90/m3u-tv/main/playlist.m3u
```

## What is included in this repository?

This repository contains a static playlist file named:

```text
playlist.m3u
```

The file contains a list of channels in standard M3U format. Each channel entry may include a channel name, internal TV metadata, group/category information, and a stream URL.

## How to use

Most applications that support M3U playlists follow a similar process:

1. Open the application settings.
2. Go to the IPTV / Live TV / Playlist / M3U section.
3. Add a new playlist source.
4. Paste this direct URL:

```text
https://raw.githubusercontent.com/il90il90/m3u-tv/main/playlist.m3u
```

5. Save the playlist.
6. Refresh or reload the channel list.

## Local usage

You can also download the playlist and use it as a local file:

```bash
curl -L -o playlist.m3u https://raw.githubusercontent.com/il90il90/m3u-tv/main/playlist.m3u
```

Then load the downloaded `playlist.m3u` file into any player or system that supports local M3U files.

## Basic M3U structure

Example channel entry:

```m3u
#EXTINF:-1 tvg-id="kan11" tvg-name="Kan 11" group-title="Israeli Broadcast",Kan 11
https://example.com/live/playlist.m3u8
```

Meaning:

- `#EXTINF` - channel metadata line.
- `tvg-id` - internal channel identifier.
- `tvg-name` - channel display name.
- `group-title` - channel group or category.
- The line below `#EXTINF` - the actual stream URL.

## Updating the playlist

The direct playlist URL does not change when `playlist.m3u` is updated in this repository.

After an update, most applications only need a playlist refresh, reload, or rescan in order to load the latest version.

## Important notes

- This is a static playlist only.
- Channels that require dynamic tokens, login sessions, cookies, signed URLs, or refresh logic are usually not suitable for a static M3U file.
- This repository does not host or stream the video content itself.
- The repository only stores a playlist file that points to external stream URLs.
- Channel availability depends on the external stream source.
- Some players may handle HLS, `.m3u8`, redirects, headers, or geo/network restrictions differently.

## Files

| File | Description |
|---|---|
| `playlist.m3u` | Main M3U playlist file for direct usage |
| `README.md` | General repository documentation and usage guide |

## Recommended usage

For the most reliable experience, use the raw GitHub URL:

```text
https://raw.githubusercontent.com/il90il90/m3u-tv/main/playlist.m3u
```

Do not use the regular GitHub file viewer URL as a playlist source. The regular GitHub page is HTML, while the raw URL returns the actual M3U file content.

## License and responsibility

Use this playlist according to your needs and in accordance with the terms of use of the external stream sources.
