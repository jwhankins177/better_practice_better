# GitHub Issues to Create

Copy and paste these into GitHub Issues at:
https://github.com/jwhankins177/better_practice_better/issues/new/choose

---

## Issue #1: Automatic Bet Settlement

**Template**: Feature Request
**Title**: [FEATURE] Automatic bet settlement from game results
**Labels**: enhancement, high priority

### Feature Description
Automatically settle pending bets by fetching final game scores/results from The Odds API and comparing them against placed bets.

### Problem it Solves
Currently, users must manually mark bets as won or lost. This requires remembering to check game results and update each bet individually, which is time-consuming and prone to errors.

### Proposed Solution
- Fetch game scores from The Odds API after games complete
- Store game IDs and bet selections when placing bets
- Periodically check pending bets against completed games
- Automatically update bet status (won/lost) based on actual results
- Update bankroll accordingly
- Notify user when bets are auto-settled

### Implementation Details
- Add "Check Results" button to manually trigger settlement
- Optionally auto-check on page load or refresh
- Handle different bet types:
  - Moneyline: Check winning team
  - Spreads: Check if team covered the spread
  - Totals: Check if total score was over/under

### Acceptance Criteria
- [ ] Fetch game scores from API
- [ ] Match pending bets to completed games
- [ ] Correctly settle moneyline bets
- [ ] Correctly settle spread bets
- [ ] Correctly settle totals (over/under) bets
- [ ] Update bankroll automatically
- [ ] Display notification of settled bets
- [ ] Handle API errors gracefully

---

## Issue #2: Parlay/Multi-Leg Betting System

**Template**: Feature Request
**Title**: [FEATURE] Parlay/multi-leg betting system
**Labels**: enhancement, high priority

### Feature Description
Allow users to combine multiple bets into a single parlay bet, where all selections must win for the parlay to pay out.

### Problem it Solves
Parlays are a popular betting strategy that offers higher payouts by combining multiple bets. Currently, users can only place individual straight bets.

### Proposed Solution
- Add "Add to Parlay" option when selecting odds
- Show parlay slip with all selected legs
- Calculate combined odds for the parlay
- Display potential payout for parlay
- Track parlay bets with individual leg status
- Show which legs won/lost/pending

### Implementation Details
- Add parlay mode toggle
- Accumulate selections before placing bet
- Calculate parlay odds: multiply decimal odds
- Store parlay structure in bet history
- Special rendering for parlay bets in history
- Allow removing legs before placing bet

### Acceptance Criteria
- [ ] Toggle between single bet and parlay mode
- [ ] Add multiple selections to parlay
- [ ] Display all parlay legs clearly
- [ ] Calculate combined odds correctly
- [ ] Show potential payout
- [ ] Place parlay bet
- [ ] Track individual leg status
- [ ] Settle parlay (all legs must win)
- [ ] Display parlay bets distinctly in history

---

## Issue #3: Advanced Statistics and Analytics

**Template**: Feature Request
**Title**: [FEATURE] Advanced statistics and analytics
**Labels**: enhancement, medium priority

### Feature Description
Expand the analytics tab with advanced betting statistics including ROI tracking, performance by bet type, time-based analysis, and odds range performance.

### Problem it Solves
Users need deeper insights into their betting performance to identify strengths, weaknesses, and patterns in their betting strategy.

### Proposed Solution
Add the following statistics to the Analytics tab:

**ROI Tracking**
- Overall ROI percentage
- ROI by sport
- ROI by bet type (moneyline, spreads, totals)

**Time-Based Analysis**
- Performance by day of week
- Performance by time of day
- Monthly performance trends

**Odds Range Analysis**
- Win rate for favorites vs underdogs
- Performance by odds ranges (-200 to -150, -150 to -110, etc.)
- Best performing odds range

**Betting Unit Tracking**
- Track bets in units (1 unit = configurable amount)
- Unit profit/loss
- Average units per bet

### Acceptance Criteria
- [ ] Calculate and display overall ROI
- [ ] Show ROI breakdown by sport
- [ ] Show ROI breakdown by bet type
- [ ] Display performance by day of week
- [ ] Show performance by time of day
- [ ] Create monthly performance chart
- [ ] Analyze performance by odds ranges
- [ ] Show favorite vs underdog performance
- [ ] Add unit tracking option
- [ ] Display unit-based statistics

---

## Issue #4: Bet History Filtering

**Template**: Improvement
**Title**: [IMPROVEMENT] Bet history filtering and search
**Labels**: enhancement, medium priority

### Current Behavior
Bet history shows all bets in chronological order with no filtering or search capabilities.

### Proposed Improvement
Add filtering and search functionality to bet history:
- Filter by status (pending/won/lost)
- Filter by sport
- Filter by date range
- Filter by bet type (moneyline/spreads/totals)
- Search by team name
- Sort by date, stake, potential win, or odds

### Benefits
- Easier to find specific bets
- Better analysis of betting patterns
- Improved user experience with large bet histories
- Quick access to pending bets only

### Implementation Notes
- Add filter controls above bet history
- Use dropdown menus and date pickers
- Add search input with live filtering
- Persist filter preferences

---

## Issue #5: Export Bet History

**Template**: Feature Request
**Title**: [FEATURE] Export bet history as CSV/JSON
**Labels**: enhancement, low priority

### Feature Description
Allow users to export their complete bet history as CSV or JSON files for external analysis or record-keeping.

### Problem it Solves
Users may want to analyze their betting data in spreadsheet applications, keep permanent records, or backup their betting history outside the app.

### Proposed Solution
- Add "Export" button in History or Settings tab
- Generate CSV file with all bet data
- Include columns: Date, Sport, Teams, Bet Type, Selection, Odds, Stake, Status, Result, Profit/Loss
- Optional: Also provide JSON export format
- Include summary statistics in export

### Acceptance Criteria
- [ ] Export button in UI
- [ ] Generate CSV with all bet data
- [ ] Include all relevant bet information
- [ ] Trigger browser download
- [ ] Format data properly (commas, quotes)
- [ ] Include summary row with totals
- [ ] Optional JSON export format

---

## Issue #6: Bet Notes and Reasoning

**Template**: Feature Request
**Title**: [FEATURE] Add notes to bets for tracking reasoning
**Labels**: enhancement, low priority

### Feature Description
Allow users to add optional notes to each bet to record their reasoning, analysis, or strategy.

### Problem it Solves
Serious bettors often want to track why they made certain bets to review their decision-making process and learn from wins and losses.

### Proposed Solution
- Add optional "Notes" field to bet slip
- Display notes in bet history
- Export notes with bet history
- Add notes to settled bets for post-analysis

### Acceptance Criteria
- [ ] Notes input field in bet slip
- [ ] Save notes with bet
- [ ] Display notes in bet history
- [ ] Edit notes after placing bet
- [ ] Include notes in CSV export

