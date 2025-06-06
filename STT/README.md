# Transcription Server Setup
> **Note:** If you open index.html directly, most browsers will show a prompt each time the recognition resets.

This document explains how to start a simple HTTP server and view real-time transcription results using Google’s WebKit API.

## Prerequisites

- Python 3.x installed on your system
- A modern web browser (Chrome, Firefox, Edge, etc.)

## Instructions

1. **Start the HTTP Server**

   Open a terminal (or command prompt) in the directory that contains ```index.html``` and run:
   ```bash
   python -m http.server 8000
   ```
   This will launch a basic HTTP server listening on port 8000.

2. **Access the Server in Your Browser**

   In your web browser, navigate to:
   ```
   http://localhost:8000/
   ```
   The directory contents (including any webpage files) will be served from the current working directory.

3. **Open Developer Tools**

   Once the page loads in your browser, press **Fn + F12** (or the appropriate key combination for your browser) to open Developer Tools. The real-time transcription results provided by Google’s WebKit API will appear in the Console tab.

> **Note:** The speech recognition session automatically restarts every 10–20 seconds. You may see short pauses or log entries indicating the restart.
