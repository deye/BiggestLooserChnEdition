# Biggest Loser CHN Edition

Weight loss tracking application for multiple participants with data analysis and visualization.

## Live Demo

View the dashboard: **https://deye.github.io/BiggestLooserChnEdition/**

## Features

- CSV-based data storage for easy tracking
- Automated calculation of weekly weight changes and total weight loss
- Individual progress tracking with trend lines
- Participant comparison visualizations
- Professional HTML dashboard with embedded charts
- Leaderboard system with rankings

## Files

- `Looser.ipynb` - Main Jupyter notebook with analysis and visualizations
- `looser_data.csv` - Data storage for participant measurements
- `index.html` - Generated HTML dashboard (view in browser or GitHub Pages)
- `.claude.md` - Project documentation and schema

## Getting Started

### Requirements

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Usage

1. **Add participant data** to `looser_data.csv` following the schema:
   - participant_id: Unique identifier
   - name: Participant name
   - date: Measurement date (YYYY-MM-DD)
   - weight_kg: Weight in kilograms
   - height_cm: Height in centimeters
   - notes: Optional notes

2. **Run the notebook** `Looser.ipynb` in Jupyter:
   ```bash
   jupyter notebook Looser.ipynb
   ```

3. **Generate dashboard** by running all cells - creates `index.html`

4. **View results** by opening the HTML file in any web browser or via GitHub Pages

## Data Schema

| Column | Type | Description |
|--------|------|-------------|
| participant_id | int | Unique identifier for each participant |
| name | string | Participant name |
| date | date | Measurement date (YYYY-MM-DD) |
| weight_kg | float | Weight in kilograms |
| height_cm | float | Height in centimeters |
| weekly_weight_change_kg | float | Auto-calculated weight change from previous week |
| total_weight_loss_kg | float | Auto-calculated total weight lost from start |
| notes | string | Optional notes |

## Dashboard Features

The HTML dashboard includes:
- Program statistics overview
- Current leader highlight
- Leaderboard with medals
- Participant summary table
- Individual progress charts with trend lines
- Comparison visualizations
- Responsive design for mobile viewing

## Tech Stack

- Python 3.x
- pandas - Data manipulation
- numpy - Numerical operations
- matplotlib - Visualization
- seaborn - Statistical visualization
- Jupyter - Interactive notebooks
