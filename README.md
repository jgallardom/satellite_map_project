# Satellite Map V4

Interactive satellite map with custom grid labeling system.

## Features

- **Grid System**: Custom coordinate grid with labels around map edges
- **Button Markers**: Every 0.5 degrees for easy navigation
- **Point Input**: Add custom coordinate points via textarea
- **Multiple Map Backgrounds**: Road, Satellite, and Topographic views
- **Label Generation**: Three different labeling systems (Alfai, 882, 882seq)
- **Coordinate Display**: Real-time mouse coordinates with 4-decimal precision

## Deployment on Render

This project is configured for deployment on Render as a static site.

### Automatic Deployment

1. **Connect Repository**: Link your GitHub repository to Render
2. **Auto-deploy**: Render will automatically detect the `render.yaml` configuration
3. **Static Site**: The service will be deployed as a static web application

### Manual Deployment

1. **Create New Service**: Choose "Static Site" in Render
2. **Build Command**: Leave empty (not needed for static sites)
3. **Publish Directory**: Set to `./templates`
4. **Root Directory**: Set to `/` (or leave default)

## Configuration

The map uses hardcoded configuration values:
- **Starting Latitude**: 8.62°N
- **Starting Longitude**: -82.00°W
- **Grid Step**: 0.01 degrees
- **Label Letters**: 23456789ABCDEFGHIJKLMNOPQRSTUVWXYZ_

## Usage

1. **Navigate**: Use the map controls or drag to move around
2. **Add Points**: Enter coordinates in the POINTS textarea and click Update
3. **View Labels**: Click anywhere on the map to see coordinate information
4. **Switch Backgrounds**: Use the layer control to change map type

## Technical Details

- **Frontend**: Pure HTML/CSS/JavaScript
- **Mapping**: Leaflet.js library
- **Grid Generation**: Custom algorithm with integer arithmetic for precision
- **Labeling**: Three different coordinate encoding systems 