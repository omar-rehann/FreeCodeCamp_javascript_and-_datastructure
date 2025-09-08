# Music Player App

A simple **Music Player App** built with **HTML, CSS, and JavaScript**.  
This project is part of a learning exercise to practice **string and array methods** by building a playlist and player controls.

## Features
- **Player Controls**:
  - Play / Pause
  - Next / Previous
  - Shuffle
- **Song Display**:
  - Shows album art
  - Displays song title and artist
- **Playlist**:
  - Songs listed in a playlist section
  - Dynamic loading of songs
- **UI Design**:
  - Modern layout with custom fonts
  - Responsive structure

## How It Works
1. Songs are stored in an array inside `main.js`.
2. When the app loads:
   - The first song’s title, artist, and album art are displayed.
   - The playlist is populated dynamically.
3. The user can:
   - Click **Play** to start the current song.
   - Use **Next** and **Previous** to switch between songs.
   - Use **Shuffle** to play a random song.
   - Click a song from the playlist to play it.

## Example UI
- Top bar shows **freeCodeCamp** branding.
- Middle section shows **album art** and **song info**.
- Bottom section displays a **playlist**.

## Requirements
- A modern browser (Chrome, Firefox, Edge).
- Internet connection for Google Fonts and external images.
- No external JavaScript libraries required.

## Possible Improvements
- Add a progress bar with current playback time.
- Allow volume control and mute/unmute.
- Store the last played song in **localStorage**.
- Add a "repeat" button for looping songs.
