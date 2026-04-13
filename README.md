# Ride Retention Analysis

**Author:** Dallen Huang

A data science challenge analyzing user demand patterns and predicting rider retention for a ride-sharing platform (Ultimate).

## Project Structure

```
├── data/
│   ├── logins.json                  # Simulated user login timestamps
│   └── ultimate_data_challenge.json # Rider cohort dataset (Jan 2014 signups)
├── ride_retention_analysis.ipynb    # Main analysis notebook
└── ride_retention_analysis.pdf      # Original challenge description
```

## Overview

This project tackles three data science problems:

### Part 1 — Exploratory Data Analysis
Analyze login timestamps from `logins.json` by aggregating them into 15-minute intervals to identify demand patterns such as daily and weekly cycles.

### Part 2 — Experiment & Metrics Design
Design an A/B experiment to evaluate whether reimbursing toll costs between the cities of Gotham and Metropolis encourages driver partners to serve both cities. Includes defining success metrics, experiment setup, and statistical validation.

### Part 3 — Predictive Modeling (Rider Retention)
Build a classification model using `ultimate_data_challenge.json` to predict whether a rider will remain active in their 6th month on the platform. The dataset includes features such as trip frequency, ratings, surge usage, and device type.

**Dataset features:**
| Feature | Description |
|---------|-------------|
| `city` | City the user signed up in |
| `phone` | Primary device |
| `signup_date` | Account registration date |
| `last_trip_date` | Date of last completed trip |
| `avg_dist` | Average trip distance (miles) in first 30 days |
| `avg_rating_by_driver` | Rider's average rating by drivers |
| `avg_rating_of_driver` | Rider's average rating of drivers |
| `surge_pct` | % of trips taken with surge multiplier > 1 |
| `avg_surge` | Average surge multiplier across all trips |
| `trips_in_first_30_days` | Number of trips in first 30 days |
| `ultimate_black_user` | Whether user took an Ultimate Black in first 30 days |
| `weekday_pct` | % of trips occurring on weekdays |

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib / seaborn
- scikit-learn
- jupyter
