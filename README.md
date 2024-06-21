
# Smart Home Device Usage Analysis

This repository contains a comprehenisve analysis of smart home device usage metrics, providing insights into user behavior, device efficiency, and preferences.

## Dataset Description

The dataset captures various metrics related to smart home device usage, including:
- Device types
- Usage patterns
- Energy consumption
- Malfunction incidents
- User satisfaction metrics

### Features

- **UserID**: Unique identifier for each user.
- **DeviceType**: Type of smart home device (e.g., Lights, Thermostat).
- **UsageHoursPerDay**: Average hours per day the device is used.
- **EnergyConsumption**: Daily energy consumption of the device (kWh).
- **UserPreferences**: User preference for device usage (0 - Low, 1 - High).
- **MalfunctionIncidents**: Number of malfunction incidents reported.
- **DeviceAgeMonths**: Age of the device in months.
- **SmartHomeEfficiency (Target Variable)**: Efficiency status of the smart home device (0 - Inefficient, 1 - Efficient).

## Analysis Overview

The analysis includes the following steps:
1. **Data Overview**: Basic statistics and structure of the dataset.
2. **Data Visualization**: Visualizing the data to understand distributions and relationships.
3. **Data Preprocessing**: Preparing the data for machine learning models.
4. **Principal Component Analysis (PCA)**: Reducing dimensionality for better visualization and model performance.
5. **Model Building**: Using RandomForestClassifier to predict device efficiency.
6. **Model Optimization**: Hyperparameter tuning using Grid Search.
7. **Model Comparison**: Comparing baseline and optimized model performances.
8. **Feature Importance**: Analyzing the significance of each feature in prediction.

## Feature Engineering

### New Features
- **EnergyPerHour**: Energy consumption per usage hour.
- **MalfunctionPerMonth**: Malfunction incidents per device age month.

### Visualizations
- Pair plots with newly created features.
- Box plots for energy consumption by device type.
- Violin plots for usage hours per day by smart home efficiency.
- Scatter plots with regression lines for energy consumption vs. usage hours.
- Correlation heatmap including new features.

## Insights and Conclusions

### Key Findings
- **Usage Patterns**: Significant variation in average usage hours per day across device types.
- **Energy Consumption**: Strong positive correlation between usage hours and energy consumption.
- **Device Efficiency**: Efficient devices consume less energy per hour.
- **Malfunction Incidents**: Higher malfunction incidents correlate with lower efficiency.
- **Feature Importance**: Energy consumption, usage hours, and malfunction incidents are key predictors of device efficiency.

### Recommendations
- **Energy Efficiency**: Focus on developing energy-efficient devices to reduce consumption and enhance user satisfaction.
- **Usage Monitoring**: Encourage optimized usage patterns to manage energy consumption effectively.
- **Reliability**: Improve device reliability to enhance efficiency and user satisfaction.
- **Future Work**: Explore the impact of user demographics and environmental factors on device usage and efficiency. Incorporate advanced machine learning models for deeper insights.

## Repository Contents

- `smart_home_device_usage_analysis.ipynb`: Jupyter notebook with the complete analysis.
- `smart_home_device_usage_data.csv`: Dataset used for the analysis.

## Getting Started

To run the analysis locally, follow these steps:

1. Clone the repository:
   ```sh
   git clone https://github.com/debjit-mandal/smart-home-device-usage-analysis.git
   ```

2. Navigate to the project directory:
   ```sh
   cd smart-home-device-usage-analysis
   ```

3. Install the required Python packages:
   ```sh
   pip install -r requirements.txt
   ```

4. Open the Jupyter notebook:
   ```sh
   jupyter notebook smart_home_device_usage_analysis.ipynb
   ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The dataset used in this analysis.
- The contributors of various Python libraries used in the analysis.

----------------------------------------------------------------

Feel free to suggest any kind of improvements.
