# chrissi's metadata remover

a lightweight, client-side tool for stripping EXIF and other metadata from your files.

## what it does

reads jpeg, png, and webp files as raw bytes and removes the metadata segments (exif, xmp, comments, thumbnails) while leaving the actual image data completely untouched. no canvas re-encoding, no quality loss, no recompression.

## features

- batch support, up to 8 files at a time, 100mb each. just a sane default to keep things fast and reliable
- optional randomized filenames
- before/after comparison when cleaning a single file, showing a few concrete examples of what was actually found (camera, gps, date taken), not the full list of everything that gets stripped

## how it works

everything runs in the browser. files are never uploaded to a server or processed anywhere else.
