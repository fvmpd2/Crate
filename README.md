# Crate

Mobile-friendly playlist builder. No installation, account, paid service, or build step required.

## Enable the website

Open https://github.com/fvmpd2/Crate/settings/pages. Under Build and deployment choose Deploy from a branch, then main and /(root), and Save. Once GitHub finishes deploying, the expected address is https://fvmpd2.github.io/Crate/.

## Import your songs

Open Library and download sample-tracks.csv as a template. Save your spreadsheet as CSV (UTF-8). Word, PDF and Excel .xlsx files are not accepted directly; export a spreadsheet as CSV first.

Required column: title. Recommended: artist. Supply either a tags column with values separated by |, or individual criteria columns such as tempo, energy, mood, vocalist, arrangement, sound source, groove, texture, era feel and setting. Custom criteria columns are supported. Use consistent spelling for values; filtering is exact.

Example:

```csv
title,artist,tempo,mood,vocalist,sound source
My Song,My Artist,Medium,Hopeful,Female,Acoustic
Another Song,Another Artist,Slow,Peaceful,Instrumental,Electronic
```

Imports add songs; a matching title and artist updates the existing entry. Remove fictional samples using the Library button if desired. The demo includes 50 fictional tracks, each with 10 vibe criteria; their tags are illustrative, not audio analysis.

## Make playlists

Choose Build a mix, clear filters, and select criteria. One value per criterion; a track must match every selection. Save the result with a name. Tracks may appear in any number of playlists. Tag edits affect future matching; saved playlists keep their original song membership.

## Laptop and phone

Open the same website on both devices. Each browser saves its own library and playlists. To transfer, choose Library > Export library on the first device, send yourself the JSON file, and import it in Library on the second. Import replaces that browser's current library. There is no automatic syncing or shared account.

## Optional audio

Import MP3s whose filenames match song titles. Audio is available for the current browser session and must be reselected after reopening. Backups include metadata and playlists, not MP3 files. Imported documents and audio stay in your browser; the app does not upload them to GitHub. Do not commit personal libraries or MP3s into this public repository.

## Development

Open index.html or serve the folder with any static web server. All application code is in index.html; no external dependencies.
