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
