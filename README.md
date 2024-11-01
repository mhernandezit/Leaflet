# NYC Subway Stations Map

This project visualizes NYC subway stations on an interactive map using Leaflet.js, styled by subway lines. The goal was to optimize JavaScript for better code readability, maintainability, and efficiency.

## Key Changes

- **Optimized Subway Line Layers**:
  - A new `createSubwayLayer` function generates map layers for each subway line, reducing redundant code.
  - Each line layer is created by specifying the color and `lineArray` (subway lines to include in the layer), making it easy to add or modify line groupings.

- **Flexible Line Matching**:
  - A helper function, `matchLine`, splits and matches station line codes, capturing all possible line combinations (e.g., "4-6-6 Express").
  - This ensures accurate mapping of all subway lines, regardless of format.