# chrissi's Metadata Remover

A lightweight, client-side tool for stripping EXIF and other metadata from your files.

## What it does

Reads JPEG, PNG, and WebP files as raw bytes and removes the metadata segments (EXIF, XMP, comments, thumbnails) while leaving the actual image data completely untouched. No canvas re-encoding, no quality loss, no recompression.

## Features

- Batch support, up to 8 files at a time, 100 MB each. Just a sane default to keep things fast and reliable
- Optional randomized filenames
- Before/after comparison when cleaning a single file, showing a few concrete examples of what was actually found (camera, GPS, date taken), not the full list of everything that gets stripped

## How it works

Everything runs in the browser. Files are never uploaded to a server or processed anywhere else.

## Design

Font: Crimson Pro (SIL Open Font License), weight 500, 18px text and 1.25em heading.

Design tokens, lavender theme. Light and dark follow the system.

| Token | Light | Dark |
| --- | --- | --- |
| background | `#faf8ff` | `#141219` |
| accent | `#211b2e` | `#efeafb` |
| body | `#4c4366` | `#b5aec8` |
| sub | `#6a6285` | `#9890b3` |
| highlight | `#ece6fb` | `#2b2638` |
