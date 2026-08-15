# Project Demo

A simple project demo for web-based automated task processing.

## Features

- **Web Server Based**: Accessible from mobile and desktop via web server
- **Schedule-Based Automatic Processing**: Automated task processing on a schedule

## Installation

```bash
comming soon..
```

## Usage

comming soon..
## Demo

### Video Split into 10MB Chunks

The demo video has been split into 7 manageable chunks (approximately 10MB each) to comply with repository size guidelines:

- `demo_chunk_00.mp4` - Chapters 0:00-10:55 (11.95 MB)
- `demo_chunk_01.mp4` - Chapters 10:55-21:52 (9.34 MB)
- `demo_chunk_02.mp4` - Chapters 21:52-32:48 (11.01 MB)
- `demo_chunk_03.mp4` - Chapters 32:48-42:23 (8.35 MB)
- `demo_chunk_04.mp4` - Chapters 42:23-52:20 (9.97 MB)
- `demo_chunk_05.mp4` - Chapters 52:20-1:01:15 (9.55 MB)
- `demo_chunk_06.mp4` - Chapters 1:01:15-10:55 (0.69 MB, end section)

**To view the complete video:**
1. Download all chunks or
2. Use the concatenation command below

### Concatenate All Chunks

```bash
# Windows (PowerShell)
Get-ChildItem -Path .\chunks\demo_chunk_*.mp4 | Sort-Object {[regex]::Match($_.Name, '\d+')} | ForEach-Object { ffmpeg -i "$_" -c copy temp.mp4 } ; ren temp.mp4 demo_full.mp4

# Or using ffmpeg directly:
ffmpeg -i "chunks/demo_chunk_%02d.mp4" -c copy demo_full.mp4
```

### Individual Chunk Preview

Each chunk can be viewed individually by clicking on the filename in the file tree, or by using:

```bash
ffplay chunks/demo_chunk_00.mp4
```
