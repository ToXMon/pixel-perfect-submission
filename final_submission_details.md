# Pixel Plus Hackathon 2025 - Final Submission

## Project: Spotify Clone with Audius API Integration and Interactive Audio Visualizer

### Live Demo
**URL:** [https://txwvtcii.manus.space](https://txwvtcii.manus.space)

### Overview
This submission is a pixel-perfect recreation of Spotify's web interface with two major enhancements:
1. Integration with the Audius API for real music streaming
2. An interactive audio visualizer with three visualization styles

### Features

#### Spotify Interface Recreation
- Dark-themed interface with correct color scheme (#121212, #181818, #1DB954)
- Sidebar with navigation and library sections
- Main content area with search and trending sections
- Player controls with progress bar and volume controls
- Responsive design that works across different screen sizes
- Exact match of Spotify's search bar with "What do you want to play?" placeholder and search icon

#### Audius API Integration
- Search functionality to find real tracks on Audius
- Display of trending tracks from the Audius platform
- Real music streaming directly from Audius servers
- Display of track artwork and artist information
- Robust error handling with fallback to mock data if API fails

#### Interactive Audio Visualizer
- Three distinct visualization styles:
  - **Bars:** Classic equalizer-style visualization
  - **Circles:** Circular pattern that pulses with the music
  - **Particles:** Dynamic particles that move based on audio intensity
- Real-time frequency analysis using Web Audio API
- Responsive canvas that adjusts to window size
- User controls to switch between visualization styles
- Accessible via the speaker icon in the player controls
- Properly renders and responds to audio with fallback mechanisms

### Technical Implementation

#### Single HTML File
As required by the hackathon rules, the entire implementation is contained in a single HTML file with inline CSS and JavaScript.

#### Key Technologies Used
- HTML5 for structure
- CSS3 for styling
- Vanilla JavaScript for functionality
- Web Audio API for audio analysis
- Canvas API for visualizations
- Fetch API for Audius integration

#### Code Organization
- HTML structure follows semantic principles
- CSS uses modern techniques like Flexbox and Grid
- JavaScript is organized into logical functions
- Error handling for API requests and audio playback
- Fallback mechanisms for when API or audio analysis fails

### How to Use

1. **Browse Trending Tracks:**
   - When you first load the page, trending tracks from Audius are displayed

2. **Search for Music:**
   - Use the search bar at the top to find tracks on Audius
   - Type your query and press Enter to search

3. **Play Music:**
   - Click on the play button on any track card to start playback
   - Use the player controls at the bottom to pause/play and adjust volume

4. **Use the Visualizer:**
   - Click the visualizer button (speaker icon) in the player controls
   - Switch between visualization styles using the buttons below the canvas
   - Close the visualizer by clicking the X in the top right

### Submission Notes

This project demonstrates:
- Pixel-perfect recreation of a complex web interface
- Integration with a third-party API
- Advanced audio processing and visualization
- Clean, well-organized code in a single HTML file
- Robust error handling and fallback mechanisms

The combination of Spotify's intuitive interface with Audius's music catalog and the custom audio visualizer creates a unique and engaging user experience that showcases both visual accuracy and technical innovation.
