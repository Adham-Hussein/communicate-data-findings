# Ford GoBike Trip Data Analysis

An exploratory data analysis project examining Bay Area bike-sharing trips in February 2019, with a focus on understanding how customers and subscribers use the service.

## Project Overview

The analysis explores trip duration, time of travel, user demographics, and differences in usage patterns between two user types:

- **Subscribers:** Registered members.
- **Customers:** Casual users.

The goal is to identify behavioral patterns that can help explain when and how different user groups use the bike-sharing service.

## Dataset

The original dataset contains **183,412 trips** and 16 columns.

It includes information such as:

- Trip duration.
- Trip start and end timestamps.
- Start and end station information.
- User type.
- User birth year.
- User gender.
- Bike-sharing membership information.

The original analysis reports a cleaned dataset of **174,884 records and 21 columns** after filtering and feature engineering.

The notebook also documents missing values in station and demographic fields. The original analysis excludes users older than 75; this filtering decision should be interpreted as an analytical assumption rather than a universal data-quality rule.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Data Preparation

The analysis includes:

1. Loading and inspecting the original dataset.
2. Checking missing values and duplicate records.
3. Converting timestamp columns to datetime.
4. Preparing categorical and numeric fields.
5. Filtering records based on the original age criterion.
6. Creating additional analytical features.

### Engineered Features

| Feature | Description |
|---|---|
| `duration_min` | Trip duration converted from seconds to minutes |
| `start_hourofday` | Hour when the trip started |
| `start_dayOfweek` | Day of the week when the trip started |
| `member_age` | Estimated member age |

## Key Findings

### 1. Subscriber Usage Patterns

Subscribers show strong weekday activity, with notable peaks around:

- 8:00 AM
- 5:00 PM

This pattern is consistent with commuting behavior.

### 2. Customer Usage Patterns

Customer trips are more concentrated in the afternoon and on weekends, suggesting a more flexible usage pattern compared with subscribers.

### 3. Weekday vs. Weekend Behavior

Subscribers use the service more heavily on working days, while customers show relatively stronger weekend activity.

### 4. Age Distribution

The original exploration reports that subscriber ages are concentrated around 28–40, while customer ages are concentrated around 18–37. The analysis also identifies a large concentration of users between 21 and 35.

## Business Interpretation

The findings suggest two different usage behaviors:

- Subscribers appear to use bike sharing more frequently for routine transportation, particularly commuting.
- Customers appear to use the service more flexibly, with greater weekend and afternoon activity.

These patterns may help a bike-sharing operator improve customer segmentation, marketing campaigns, and service planning.

## Repository Contents

| File | Description |
|---|---|
| `201902-fordgobike_exploration.ipynb` | Jupyter Notebook containing the exploratory analysis |
| `201902-fordgobike_exploration.html` | HTML export of the analysis |
| `Slide_desk_201902-fordgobike_exploration.slides.html` | Presentation export |
| `README.md` | Project documentation |

## How to Explore the Project

Open the notebook:

```bash
jupyter notebook 201902-fordgobike_exploration.ipynb
```

Install the main dependencies if they are not already available:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## Limitations and Further Work

- Validate the age-filtering assumption and its impact on the results.
- Document how missing demographic values are handled.
- Reconcile the reported row and column counts with the final notebook output.
- Compare trip duration distributions across user types.
- Investigate station-level demand and seasonal patterns.
- Add reproducible environment and data-source instructions.

## Project Status

Exploratory data analysis completed in a Jupyter Notebook. The findings represent patterns in the February 2019 dataset and should not automatically be generalized to other periods.
