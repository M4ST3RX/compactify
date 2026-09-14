# Compactify

A lightweight Windows desktop utility that compresses game folders using the built-in NTFS `compact.exe` with LZX compression, and restores them on demand.

## Download

Get the latest release from the [`publish/v1.0`](publish/v1.0)

## Features

- Scan installed games from Steam and other launchers
- Compress or restore individual games with one click
- Queue multiple games and process them in the background
- Scheduler with idle detection and a daily time window
- Live progress and per-game savings stats
- Minimize to system tray

## Usage

1. Run `Compactify.exe`.
2. Select a game and click the compress or restore icon.
3. Switch to the Queue tab to watch progress.

## Requirements

- Windows 10/11
- NTFS drive

## Notes

- Compression is done with `compact.exe /EXE:LZX`.
- The executable is not code-signed, so Windows may show a SmartScreen warning on first run. Click **More info** → **Run anyway** if you trust the file.

## Version

v1.0.0
