---
name: yt-dlp
description: Download videos from YouTube and 1000+ other sites using yt-dlp. Use this when the user asks to download, save, or grab videos from any supported site including YouTube, Bilibili, Vimeo, Twitter, etc.
---

# yt-dlp Video Downloader

Download videos using yt-dlp. Simply provide a video URL and the tool will download it.

## Quick Start

```bash
yt-dlp "VIDEO_URL"
```

The video will be saved to the current directory with its original title.

## Common Options

### Specify output directory
```bash
yt-dlp -o "PATH/%(title)s.%(ext)s" "VIDEO_URL"
```

### Download best quality
```bash
yt-dlp -f "bestvideo+bestaudio/best" "VIDEO_URL"
```

### Download audio only (MP3)
```bash
yt-dlp -x --audio-format mp3 "VIDEO_URL"
```

### Download specific format (MP4)
```bash
yt-dlp -f "bestvideo[ext=mp4]+bestaudio[ext=m4a]/best[ext=mp4]/best" "VIDEO_URL"
```

### List available formats first
```bash
yt-dlp -F "VIDEO_URL"
```

## Notes

- yt-dlp supports 1000+ websites including YouTube, Bilibili, Vimeo, Twitter, Instagram, etc.
- FFmpeg is recommended for merging video/audio streams (install separately if needed)
- Use `yt-dlp --help` for more options
