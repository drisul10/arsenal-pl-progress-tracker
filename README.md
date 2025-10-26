# Arsenal Premier League Progress Tracker 🔴⚪

A comprehensive dashboard that tracks and compares Arsenal's Premier League performance across multiple seasons (2022/23 - 2025/26) with interactive visualizations and detailed match analysis.

## ✨ Features

- **Multi-Season Comparison**: Track Arsenal's progress across 4 seasons simultaneously
- **Interactive Charts**: Visualize cumulative points, goals scored/conceded with Chart.js
- **Matchday Analysis**: Detailed matchday-by-matchday results comparison
- **Real-time Statistics**: Dynamic stats including wins, draws, losses, goals, and goal difference
- **Responsive Design**: Mobile-first design with TailwindCSS
- **Modern UI**: Clean, gradient-based interface with Arsenal's brand colors

## 🚀 Live Demo

**🌐 GitHub Pages**: [View Live Dashboard](https://drisul10.github.io/arsenal-pl-progress-tracker)

**📱 Local Development**: Open `index.html` in your browser to view locally.

## 📊 Dashboard Components

### 1. Season Statistics Cards
- Current points total for each season
- Goals for/against and goal difference
- Color-coded by season for easy identification

### 2. Interactive Charts
- **Cumulative Points Progress**: Line chart tracking points accumulation
- **Goals Scored (GF)**: Bar chart comparing goals scored per season
- **Goals Conceded (GA)**: Bar chart comparing defensive performance
- **Goals Comparison**: Side-by-side comparison of offensive vs defensive stats

### 3. Data Tables
- **Match Results**: Complete matchday-by-matchday results
- **Season Summary**: Comprehensive statistics breakdown

## 🔧 Setup

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd arsenal-pl-progress-tracker
   ```

2. **Open the dashboard**
   ```bash
   # Simply open index.html in your browser
   open index.html
   # or
   python -m http.server 8000  # For local server
   ```

3. **View the dashboard**
   - Navigate to `http://localhost:8000` (if using local server)
   - Or open `index.html` directly in your browser

## 🌐 GitHub Pages Deployment

### Automatic Deployment (Recommended)

This project includes a GitHub Actions workflow for automatic deployment to GitHub Pages:

1. **Push to GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Navigate to **Settings** → **Pages**
   - Under **Source**, select **GitHub Actions**
   - The deployment will start automatically

3. **Access your live site**
   - Your dashboard will be available at: `https://drisul10.github.io/arsenal-pl-progress-tracker`
   - Replace `drisul10` with your actual GitHub username

### Manual Deployment

If you prefer manual deployment:

1. **Enable GitHub Pages**
   - Go to **Settings** → **Pages** in your repository
   - Under **Source**, select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

2. **Access your site**
   - Your site will be available at the same URL format
   - Updates will deploy automatically when you push to main

### ✅ GitHub Pages Checklist

- [ ] Repository is public (or you have GitHub Pro/Team)
- [ ] `index.html` is in the root directory ✅
- [ ] All assets use relative paths ✅
- [ ] External dependencies are CDN-based ✅
- [ ] GitHub Pages is enabled in repository settings

## 📁 Project Structure

```
arsenal-pl-progress-tracker/
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Pages deployment workflow
├── data/
│   └── arsenal-data.json    # Match data and statistics
├── index.html              # Main dashboard HTML
├── .nojekyll               # Disable Jekyll processing
├── README.md               # This file
└── .gitignore             # Git ignore file
```

## 📊 Data Structure

The `arsenal-data.json` file contains:
- **Match Results**: Detailed scores and statistics for each matchday
- **Season Information**: Color coding and season identifiers
- **Completion Status**: Tracks which matches have been played
- **Last Updated**: Timestamp for data freshness

### Example Match Entry
```json
{
  "matchday": 1,
  "opponent": "Manchester United",
  "venue": "A",
  "results": {
    "2022/2023": {
      "score": "3-1",
      "arsenalGoals": 1,
      "opponentGoals": 3
    },
    // ... other seasons
  }
}
```

## 🎨 Technologies Used

- **HTML5** - Structure and semantic markup
- **TailwindCSS** - Responsive styling and components
- **Chart.js** - Interactive data visualizations
- **Vanilla JavaScript** - Data processing and DOM manipulation

## 📈 Key Metrics Tracked

- **Points**: 3 for wins, 1 for draws, 0 for losses
- **Goals For (GF)**: Total goals scored
- **Goals Against (GA)**: Total goals conceded
- **Goal Difference (GD)**: GF - GA
- **Win/Draw/Loss Record**: Complete match outcomes

## 📅 Data Sources

Match data is sourced from FBRef.com:
- [2025-2026 Season](https://fbref.com/en/squads/18bb7c10/2025-2026/matchlogs/c9/schedule/Arsenal-Scores-and-Fixtures-Premier-League)
- [2024-2025 Season](https://fbref.com/en/squads/18bb7c10/2024-2025/matchlogs/c9/schedule/Arsenal-Scores-and-Fixtures-Premier-League)
- [2023-2024 Season](https://fbref.com/en/squads/18bb7c10/2023-2024/matchlogs/c9/schedule/Arsenal-Scores-and-Fixtures-Premier-League)
- [2022-2023 Season](https://fbref.com/en/squads/18bb7c10/2022-2023/matchlogs/c9/schedule/Arsenal-Scores-and-Fixtures-Premier-League)

## 🔄 Updating Data

To update the match data:
1. Edit `data/arsenal-data.json`
2. Update match results with new scores
3. Increment `completedMatchday` as needed
4. Update `lastUpdated` timestamp

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 👨‍💻 Creator

**Andri Sul**
- Twitter: [@drisul10](https://twitter.com/drisul10)

---

*Last updated: October 2025*