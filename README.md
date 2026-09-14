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

## Virus Scan
 
[![VirusTotal scan](https://img.shields.io/badge/VirusTotal-View%20report-4285F4?logo=virustotal&logoColor=white)](https://www.virustotal.com/gui/file/b2eedbd62a663120cfdc5dc11516e749262206a76abeb3359e69e6f11b95567a/detection)

Compactify may be flagged by one obscure AV engine as `W32.Malware.F3354589` — this is a false positive caused by the app enumerating running processes and invoking `compact.exe`. The source is private, but the behavior is fully explained above.

## Notes

- Compression is done with `compact.exe /EXE:LZX`.
- The executable is not code-signed, so Windows may show a SmartScreen warning on first run. Click **More info** → **Run anyway** if you trust the file.

## Version

v1.0.0
