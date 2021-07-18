# photo-importer
Script to import and archive photos &amp; videos

This script looks for images and videos in the current directory, extracts the date from the EXIF
data, and moves them into specified directories according to the date.

## Usage

```
photo-importer [options]
```

Where options may include:

### `-q --(no-)quiet`
Run in quiet mode
### `--(no-)dry-run`
Run in dry run mode - don't move any files
### `--source`
Specify where to look for photos and videos. Defaults to current working directory.
### `-p --photo-path`
Specify destination directory to move photos to. Defaults to `~/Pictures/Photos`
### `-v --video-path`
Specify destination directory to move videos to. Defaults to `~/Videos/Clips`
### `-m --month`
Group photos in directories by month, instead of by day

These options may be passed in on the command line or set in a config file `~/.photo-importer.conf`.
If options are set in multiple places, the order of inheritance is:

1. command line
1. config file
1. defaults
