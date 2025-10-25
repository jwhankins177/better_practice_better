# Better Practice Bets - Development Branch

A practice betting application with live odds integration, cloud sync, and comprehensive analytics.

## Features
- Live odds from The Odds API for NFL, NBA, NHL, MLB, EPL, NCAAB, NCAAF
- Multiple betting markets: Moneyline, Point Spreads, Totals (Over/Under)
- Cloud synchronization via Firebase Firestore
- Quick bet amount presets and percentage-based betting
- Betting streak tracking
- Performance analytics with interactive charts
- Mobile-responsive design

## Development Changelog

### v1.4.0 - In Development (October 25, 2025)
**New Features:**
- ✅ Quick bet amount buttons ($25, $50, $100, $250, 1%, 2%, 5% of bankroll)
- ✅ Betting streak tracker (current streak, best win/loss streaks)
- ✅ Performance charts and analytics tab with Chart.js visualizations
  - Bankroll progression over time
  - Win rate by sport
  - Performance statistics grid (avg win/loss, biggest win/loss, avg stake)

**In Progress:**
- 🚧 Parlay/multi-leg betting system
- 🚧 Advanced statistics (ROI, time-based analysis, odds range performance)

### v1.3.0 - Current Production (October 2025)
**Features:**
- Multiple betting markets (Moneyline, Spreads, Totals)
- API key configuration in settings tab
- Cloud sync with Firebase Firestore
- 7-day game window
- Mobile-responsive layout
- iOS formatting fixes

**Bug Fixes:**
- Fixed betting interface freeze when clicking invalid odds
- Fixed NaN display issues with unavailable markets
- Removed overlapping text on iOS devices

### v1.2.0 (October 2025)
**Features:**
- Added GitHub Pages deployment
- Implemented CORS proxy for mobile access
- Cloud synchronization across devices

### v1.1.0 (October 2025)
**Features:**
- Settings tab with API key management
- Multiple betting market support (h2h, spreads, totals)
- Market toggle UI

### v1.0.0 (October 2025)
**Initial Release:**
- Basic betting interface with moneyline odds
- Bankroll management ($1000 starting)
- Bet history tracking
- Sport selector (NFL, NBA, NHL, MLB, EPL, NCAAB, NCAAF)
- Local storage persistence

## Tech Stack
- HTML/CSS/JavaScript (Single Page Application)
- Firebase Firestore (Cloud Storage)
- The Odds API (Live Odds Data)
- Chart.js (Data Visualization)
- GitHub Pages (Hosting)

## Setup
1. Clone the repository
2. Add your Odds API key in the Settings tab
3. Open `index.html` in a browser or visit the GitHub Pages deployment

## API Configuration
Get a free API key from [The Odds API](https://the-odds-api.com/)

## Branch Strategy
- `main` - Production-ready code
- `development` - Active feature development

## Contributing
Features are developed on the `development` branch and merged to `main` when stable.
