# ExifTool

**Category:** Metadata

**Purpose:** Read, write, and edit metadata embedded in images, documents, audio, and video files (EXIF, IPTC, XMP, and many other formats).

**Official Repository:** [github.com/exiftool/exiftool](https://github.com/exiftool/exiftool)

**Website:** [exiftool.org](https://exiftool.org)

**Status:** ✅ Active | **License:** GPL-3.0 / Artistic (dual)

**Installation:**

```bash
# Debian/Kali/Ubuntu
sudo apt install libimage-exiftool-perl

# or from source/website
```

**Basic Usage:**

```bash
exiftool file.jpg
```

**Example:**

```bash
exiftool -gps:all -createdate photo.jpg
```

**What it is useful for:**

- Extracting camera model, timestamps, GPS coordinates, and authorship metadata from files obtained directly (not re-uploaded to social media).
- Verifying whether a claimed capture date/location for an image is plausible.
- Stripping or editing metadata before sharing files (privacy hygiene).

**Limitations:**

- Most major social platforms strip EXIF/GPS metadata on upload — this tool is most useful on originals, not downloaded social-media copies.
- Metadata can be edited or forged, so it should be treated as a lead requiring corroboration, not standalone proof.
- Missing metadata does not confirm anything — many cameras/apps omit GPS by default.

**Operational Safety:**

ExifTool runs entirely locally — no data leaves your machine, making it the preferred choice over web-based "metadata viewer" services for sensitive files (see [OPSEC](../../docs/opsec.md)).
