# MyStravaStats

MyStravaStats is a personal data analysis project built using Jupyter Notebook and Python to visualize and understand personal fitness trends using exported Strava activity data. This project offers comprehensive insights through interactive plots and statistics for various types of activities (running, cycling, hiking, etc.).

## Insights You Can Discover

- Are you improving your speed or distance over time?
- Which days of the week are you most active?
- Are there patterns in your activity start times?
- What type of activity do you perform most often?
- Which regions (e.g., USA vs. Poland) are most common for your rides?
- Are there seasonal trends in your activity levels?

## Features

- **Activity Summary**: View total activities, duration, and distance metrics.
- **Monthly and Weekly Trends**: Track your pace, speed, and distance over time.
- **Heatmaps**: Visualize what times and days you're most active.
- **Streaks & Rest Days**: Identify your longest streaks and recovery periods.
- **Activity Frequency**: Analyze how often you work out each day of the week.
- **Pie Charts**: See your most common types of workouts.
- **Time Zone Support**: Adjusts timestamps to your local time (e.g., EST).

## Project Structure

```plaintext    
├── plots/
│   ├── activities_per_weekday.png
│   ├── activity_start_times_heatmap.png
│   ├── all_activities_pi_chart_distribution.png
│   ├── correlation_heatmap.png
│   ├── interactive_routes_clean.html
│   ├── interactive_routes_detailed.html
│   ├── monthly_average_speed.png
│   ├── monthly_distance.png
│   ├── monthly_elevation_gain.png
│   ├── monthly_moving_hours.png
│   ├── poland_activities.png
│   ├── power_output_per_ride.png
│   ├── power_zone_frequency.png
│   ├── usa_activities.png
│   ├── weekly_average_speed.png
│   ├── weekly_distance.png
│   ├── weekly_elevation_gain.png
│   └── weekly_moving_hours.png
├── strava_analysis.ipynb
├── strava_activities.csv      
├── power_zone_summary.csv              
└── README.md
```

## Setup Instructions

### Prerequisites

Ensure you have the following installed:

- Python 3.7+
- Jupyter Notebook or Jupyter Lab

You can install the required Python packages using:

```bash
pip install webbrowser pandas geopandas numpy matplotlib polyline folium pathlib seaborn
```

## Customization Tips

- To change the time zone, update the `.tz_convert()` line in the notebook.
- You can filter activities by type (e.g., only cycling) by modifying the DataFrame filters.
- Add support for other visualizations like heart rate, calories burned, or elevation.
- Customize plots with your preferred color schemes or styles using Matplotlib/Seaborn options.

## Data Privacy

Your Strava data remains local and is never uploaded or shared. If publishing this notebook, make sure to remove or anonymize sensitive data such as location details or GPX files.

## Sample Plots

### Activity Frequency Heatmap
![Heatmap](plots/activity_start_times_heatmap.png)

### Weekly Distance Overview
![Monthly Distance](plots/weekly_distance.png)

### Common Workouts
![Monthly Distance](plots/all_activities_pi_chart_distribution.png)

### Locations of Activities 
![USA Activities](plots/usa_rides.png)
![Poland Activities](plots/poland_activities.png)

## Map Visualizations

This project includes interactive HTML maps for route visualizations:

- `interactive_routes_clean.html`: Simplified visual of GPS routes.
- `interactive_routes_detailed.html`: Detailed map view of rides.

### Interactive Clean Map

![Clean Map](plots/interactive_clean.png)

### Interactive Detailed Map

![Detailed Map](plots/interactive_detailed.png)

## Limitations and Future Improvements

- Currently supports only activities with GPS data.
- Does not include heart rate or power data (yet).
- Future plans:
  - Add performance trendlines and forecast models.
  - Implement goal tracking and achievement detection.
  - Enable comparisons between years.
