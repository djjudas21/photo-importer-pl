# photo-importer
Script to import and archive photos &amp; videos

This script looks for images and videos in the current directory, extracts the date from the EXIF
data, and moves them into specified directories according to the date.

## Usage

```
photo-importer [options]
```

Where options may include:

### `--(no-)verbose`
Run in verbose mode. Default: true
### `--(no-)dry-run`
Run in dry run mode - don't move any files
### `--source`
Specify where to look for photos and videos. Defaults to current working directory.
### `-p --photo-path`
Specify destination directory to move photos to. Defaults to `/home/jonathan/Pictures/Photos`
### `-v --video-path`
Specify destination directory to move videos to. Defaults to `/home/jonathan/Videos/Clips`
