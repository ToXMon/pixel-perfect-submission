# ResonateWeb3 - ML-Powered Decentralized Music Streaming

A decentralized music streaming platform built with the Audius API, ResonateWeb3 reimagines music discovery using blockchain technology and machine learning. This web3-native Spotify clone eliminates intermediaries by streaming directly from Audius' peer-to-peer network, giving artists full ownership of their work and fans transparent access. 

## 🎯 Key Features

### 🎵 Core Music Features
- **Decentralized Streaming**: Stream directly from Audius' peer-to-peer network
- **Immersive Audio Visualizer**: Real-time audio visualization with multiple modes (Bars, Circles, Particles)
- **Modern Interface**: Clean, Spotify-inspired design with responsive layout
- **Search & Discovery**: Find tracks, artists, and trending music

### 🤖 Machine Learning Features

#### 1. **Intelligent Search with TF-IDF Ranking**
- Semantic search that understands context and relevance
- Ranks results based on query relevance, user preferences, and popularity
- Goes beyond simple keyword matching to find the best matches

#### 2. **Personalized Recommendations ("For You")**
- Collaborative filtering based on your listening history
- Learns your preferences for genres, artists, and moods
- Improves recommendations as you listen to more tracks
- Cold start handling: Shows trending tracks for new users

#### 3. **Mood-Based Discovery**
Six mood categories powered by ML:
- ⚡ **Energetic**: Upbeat, dance, electronic tracks
- 😌 **Chill**: Ambient, lofi, downtempo music
- 🎯 **Focus**: Instrumental, classical, study music
- 💪 **Workout**: High-energy rock, hip-hop, EDM
- 😊 **Happy**: Pop, indie, feel-good tracks
- 😢 **Sad**: Acoustic, emotional, ballads

#### 4. **Content-Based Filtering**
- Finds similar tracks based on multiple factors:
  - Genre similarity (30% weight)
  - Mood matching (20% weight)
  - Artist connection (25% weight)
  - Title similarity using Jaccard coefficient (25% weight)

#### 5. **Smart Playlist Generation**
- Creates coherent playlists from a seed track
- Uses similarity algorithms to find related songs
- Adds variety with controlled randomness
- Generates 15-track playlists automatically

#### 6. **Learning System**
- Tracks your listening history (last 100 plays)
- Builds a user preference profile:
  - Genre preferences with weighted scores
  - Favorite artists tracking
  - Mood preference analysis
- Stores data locally using localStorage
- Privacy-focused: All data stays on your device

#### 7. **Listening Statistics Dashboard**
- Total plays counter
- Unique tracks listened to
- Top 3 genres
- Top 3 artists
- Visual stats cards with real-time updates

### 🎨 User Experience Enhancements
- **ML Discovery Section**: Dedicated sidebar menu for ML features
- **Similar Tracks Button**: Hover over any track to find similar music
- **Visual Mood Cards**: Color-coded, emoji-enhanced mood selection
- **Dynamic Headers**: Context-aware page titles
- **Responsive Design**: Works seamlessly on desktop and mobile
- **Demo Mode**: Graceful fallback with mock data when API is unavailable

## 🚀 Technology Stack

- **Frontend**: Vanilla JavaScript (ES6+), HTML5, CSS3
- **API**: Audius Decentralized Music Protocol
- **ML Algorithms**:
  - TF-IDF (Term Frequency-Inverse Document Frequency) for search ranking
  - Collaborative Filtering for personalized recommendations
  - Content-Based Filtering for similarity matching
  - Jaccard Similarity for text comparison
- **Data Storage**: localStorage for user preferences and history
- **Audio Processing**: Web Audio API with visualizer

## 🎓 Machine Learning Implementation Details

### TF-IDF Search Ranking
```javascript
// Tokenizes queries and track metadata
// Calculates term frequency in track text
// Combines with personalization and popularity scores
// Returns ranked results with weighted scoring (60% TF-IDF, 30% personal, 10% popularity)
```

### Collaborative Filtering
```javascript
// Analyzes listening history to build user profile
// Scores tracks based on:
//   - Genre preference (40% weight)
//   - Artist preference (35% weight)
//   - Mood preference (25% weight)
//   - Recency bonus (10% weight)
//   - Popularity factor (5% weight)
```

### Content Similarity Algorithm
```javascript
// Calculates similarity between two tracks:
//   - Exact genre match: +0.3
//   - Mood match: +0.2
//   - Same artist: +0.25
//   - Title word overlap (Jaccard): up to +0.25
// Results cached for performance
```

## 📊 How the ML Learns

1. **Play a track** → System records: trackId, title, artist, genre, mood, timestamp
2. **Build profile** → Updates genre, artist, and mood preference counters
3. **Generate recommendations** → Scores all tracks based on your profile
4. **Rank search results** → Combines relevance with your preferences
5. **Discover similar tracks** → Uses content-based filtering on track metadata

## 🎮 Usage

1. **Browse Trending**: Start with popular tracks from the Audius network
2. **Search**: Use the search bar with ML-powered ranking
3. **Explore Moods**: Click mood cards to discover music by feeling
4. **Get Recommendations**: Visit "For You" for personalized suggestions
5. **Find Similar**: Hover over tracks and click the info button for similar music
6. **Generate Playlists**: Create automatic playlists from any track
7. **Track Stats**: View your listening statistics in "Your Stats"

## 🔧 Setup

Simply open `index.html` in a modern web browser. No build process required!

The application will:
- Attempt to connect to Audius API
- Fall back to demo mode if API is unavailable
- Start learning from your first played track

## 🌐 Demo Mode

When external APIs are blocked (e.g., in sandboxed environments), the app runs in demo mode with:
- 12 diverse mock tracks across multiple genres
- All ML features fully functional
- Complete user experience demonstration

## 🎨 Design Philosophy

As a world-class product designer, the interface prioritizes:
- **Discoverability**: ML features prominently displayed
- **Visual Hierarchy**: Clear information architecture
- **Feedback**: Real-time updates and statistics
- **Delight**: Smooth animations and emoji-enhanced UI
- **Accessibility**: Clear labels and intuitive navigation

## 🔒 Privacy

- All learning data stored locally (localStorage)
- No external tracking or analytics
- User preference data never leaves your device
- Fully transparent ML algorithms

## 🚀 Future Enhancements

- Deep learning models for audio feature extraction
- Artist recommendation networks
- Social collaborative filtering
- Real-time trending analysis
- Playlist continuation algorithms
- Cross-session learning with optional cloud sync

---

Built with ❤️ for decentralized music discovery and machine learning
