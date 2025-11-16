# SVG Presenter

A simple tool for presenting slides from an Inkscape SVG file.

## Usage

- Open `index.html` in a browser
- Select your SVG file
- Navigate with arrow keys: ← → to move between slides, ↑ to toggle zoom
- Click anywhere to enter fullscreen mode
- In zoomed-out view, click on a slide to jump to it

## How it works

- Finds all top-level `<g>` elements within the root Inkscape layer
- Filters out empty slides (zero width/height)
- Sorts slides by column (left to right), then top to bottom within each column
- Displays each slide fullscreen with aspect ratio preserved
- Auto-reloads the file every 250ms to show live updates from Inkscape
