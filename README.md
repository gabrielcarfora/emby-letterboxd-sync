# emby-letterboxd-sync

A Python script that synchronises Letterboxd watchlists with Emby. Automatically creates and updates Emby playlists based on defined Letterboxd watchlists.

## Features

- Supports multiple Emby/Letterboxd users.
- Runs in single-sync or daemon mode.

## Requirements

- Python 3.10+
- Emby server with API access
- Letterboxd account(s)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/gabrielcarfora/emby-letterboxd-sync.git
cd emby-letterboxd-sync
```

2. Run the setup:
```bash
python3 letterboxd_sync.py -s
```

This creates a virtual environment and installs required dependencies automatically.

## Configuration

During setup, you'll need to provide:
- Emby server URL (e.g., http://your.emby.ip.address:8096)
- Emby API key
- Sync interval (in milliseconds)

## Usage

Add a new user:
```bash
python3 letterboxd_sync.py -a
```

Run a single sync:
```bash
python3 letterboxd_sync.py -r
```

Run in daemon mode:
```bash
python3 letterboxd_sync.py -d
```

Show help:
```bash
python3 letterboxd_sync.py -h
```
