# Jellyfin Desktop (Personal Fork)

Personal Windows x64 build of [jellyfin/jellyfin-desktop](https://github.com/jellyfin/jellyfin-desktop) with cherry-picked PRs and local fixes.

## Merged PRs
- #346 — Improve Dolby Vision handling on Windows
- #360 — Fix mouse and context menu offset on HiDPI displays
- #363 — Window scale fixes; Context menu visibility fixes

## Local Fixes
- Use `SetPropertyStringAsync` instead of `SetOptionString` for `target-colorspace-hint` (post-init option setting is a no-op in mpv)
- DV detection checks specific codec fields (`Codec`, `CodecTag`, `Container`) instead of full JSON blob to avoid false positives

## Build

Windows x64 only, via GitHub Actions on this fork.
