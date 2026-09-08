# MediaInfo

**Category:** Metadata

**Purpose:** Display technical and tag metadata for audio and video files (codec, duration, bitrate, encoder, embedded tags).

**Official Repository:** [github.com/MediaArea/MediaInfo](https://github.com/MediaArea/MediaInfo)

**Website:** [mediaarea.net/en/MediaInfo](https://mediaarea.net/en/MediaInfo)

**Status:** ✅ Active | **License:** BSD-2-Clause

**Installation:**

```bash
# Debian/Kali/Ubuntu
sudo apt install mediainfo
```

**Basic Usage:**

```bash
mediainfo video.mp4
```

**Example:**

```bash
mediainfo --Output=JSON video.mp4 > metadata.json
```

**What it is useful for:**

- Identifying the encoder/software used to produce a video or audio file, which can help assess authenticity or origin.
- Extracting technical details for verification workflows (e.g., comparing multiple copies of the same file for re-encoding signs).

**Limitations:**

- Like all metadata tools, results reflect what the file's metadata *claims* — this can be stripped, edited, or absent.
- Most platforms re-encode uploaded media, removing original metadata.

**Operational Safety:**

Runs entirely locally — no data leaves your machine, which is preferable for sensitive files over uploading to a web-based metadata viewer.
