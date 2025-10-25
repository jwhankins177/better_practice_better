# Better Practice Bets

A practice betting application with live sports odds, cloud synchronization, and performance analytics.

🔗 **Live App:** https://jwhankins177.github.io/better_practice_better

## Features
- 📊 Live odds from The Odds API for 7 sports (NFL, NBA, NHL, MLB, EPL, NCAAB, NCAAF)
- 🎯 Multiple betting markets: Moneyline, Point Spreads, Totals (Over/Under)
- ☁️ Cloud synchronization via Firebase Firestore - access your bets from any device
- 💰 Quick bet presets and percentage-based betting
- 📈 Performance analytics with interactive charts
- 📱 Mobile-responsive design
- 🔥 Betting streak tracking

## Getting Started
1. Visit https://jwhankins177.github.io/better_practice_better
2. Get a free API key from [The Odds API](https://the-odds-api.com/)
3. Enter your API key in the Settings tab
4. Start practicing your betting strategy with a $1000 bankroll!

## How It Works
- **Practice Mode:** No real money involved - perfect for testing strategies
- **Cloud Sync:** Your bankroll and bet history sync across all your devices
- **Live Odds:** Real-time odds from professional sportsbooks
- **Analytics:** Track your performance with detailed charts and statistics

## Production Changelog

### v1.5.0 - Latest Release (October 25, 2025)
**Improvements:**
- ⚡ Instant bet placement - removed confirmation modal for faster workflow
- 🗑️ Delete pending bets - refunds stake and removes bet from history
- 🎯 Spreads set as default betting market
- 🔧 Debug info moved to Settings tab for cleaner interface

### v1.4.0 (October 25, 2025)
**New Features:**
- ✨ Quick bet amount buttons ($25, $50, $100, $250) and percentage presets (1%, 2%, 5%)
- 🔥 Betting streak tracker showing current streak and best/worst streaks
- 📊 Performance analytics tab with Chart.js visualizations:
  - Bankroll progression over time
  - Win rate analysis by sport
  - Performance statistics (avg win/loss, biggest wins/losses, avg stake)

### v1.3.0 (October 2025)
**Features:**
- Added multiple betting markets (Moneyline, Point Spreads, Totals)
- API key configuration moved to settings tab
- Cloud synchronization with Firebase Firestore
- 7-day game window for upcoming matches
- Mobile-responsive layout improvements
- iOS device formatting fixes

**Bug Fixes:**
- Fixed betting interface freeze with invalid odds
- Fixed NaN display for unavailable markets
- Removed overlapping UI elements on mobile

### v1.2.0 (October 2025)
- GitHub Pages deployment
- CORS proxy implementation for mobile compatibility
- Cross-device cloud synchronization

### v1.1.0 (October 2025)
- Settings tab with API key management
- Multiple betting market support
- Market toggle interface

### v1.0.0 (October 2025)
**Initial Release:**
- Basic betting interface with moneyline odds
- Bankroll management ($1000 starting balance)
- Bet history tracking
- 7 sport leagues supported
- Local storage persistence

## Tech Stack
- **Frontend:** HTML/CSS/JavaScript (Vanilla JS)
- **Database:** Firebase Firestore
- **API:** The Odds API
- **Charts:** Chart.js v4.4.0
- **Hosting:** GitHub Pages

## Contributing
We welcome contributions! Please see our [Contributing Guidelines](CONTRIBUTING.md) for details on:
- Development workflow
- Branch strategy
- Code style
- Pull request process

**Quick Links:**
- 📋 [Development Guide](DEV_GUIDE.md) - Quick reference for daily workflow
- 🗺️ [Roadmap](ROADMAP.md) - Feature roadmap and priorities
- 🐛 [Report a Bug](https://github.com/jwhankins177/better_practice_better/issues/new?template=bug_report.md)
- 💡 [Request a Feature](https://github.com/jwhankins177/better_practice_better/issues/new?template=feature_request.md)

## Development
Active development happens on feature branches that are merged into `main` via pull requests.

### Branch Structure
- `main` - Production releases (stable, always deployable)
- `feature/*` - Feature branches (created as needed, deleted after merge)

## Support
For issues or feature requests, please create an issue on GitHub.

## License
MIT License - Free to use for practice and educational purposes.
