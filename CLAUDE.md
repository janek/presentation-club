# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a simple static website for "Presentation Club" that displays a square video with a download link for a presentation file. The entire application is contained in a single HTML file with embedded CSS and JavaScript.

## Architecture

- **Single-file architecture**: All code is contained in `index.html`
- **Static assets**: 
  - `output_video.mp4`: Main presentation video
  - `p.key`: Keynote presentation file for download
  - `favicon.svg`: Site favicon
- **No build system**: Direct HTML/CSS/JavaScript with no compilation needed
- **Responsive design**: Square video that adapts to mobile screens

## Development

Since this is a static HTML file with no build process:
- Open `index.html` directly in a browser to view changes
- Use a local server for development: `python -m http.server 8000` or any static file server
- No compilation, bundling, or package management required

## Key Features

- Video loading with opacity transition and loader overlay
- Responsive square video container (600x600px on desktop, full viewport width on mobile)
- Fixed download button for the Keynote file
- Clean, minimal white background design

## File Structure

```
/
├── index.html          # Main application file (HTML/CSS/JS)
├── output_video.mp4    # Presentation video
├── p.key              # Downloadable Keynote presentation
└── favicon.svg        # Site icon
```