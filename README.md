# Vidiana update metadata

Vidiana reads `version.json` from `main` (Help > Check for updates) and downloads the patch
installer named in `url` from this repository's GitHub releases.

When publishing a release:

1. Build `vidiana_patch.exe` with `d:\dev\installer\vidiana\build_setup.bat`.
2. Create a release `v<version>` here and attach `vidiana_patch.exe`.
3. Update `version`, `date`, `notes_ko`, `notes_en`, `url`, and `sha256` (SHA-256 of the attached file) in `version.json`.

Keep every `notes*` value on a single line. Do not use `\n` escapes inside those strings.
