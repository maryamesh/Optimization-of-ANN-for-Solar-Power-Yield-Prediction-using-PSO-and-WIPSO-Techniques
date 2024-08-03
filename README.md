![image](https://github.com/user-attachments/assets/ada3d310-797f-4e91-a96a-b0ade3e94d4b)

# Optimization of ANN for Solar Power Yield Prediction

## Abstract
This research explores optimizing an Artificial Neural Network (ANN) using Particle Swarm Optimization (PSO) and Weighted Improved Particle Swarm Optimization (WIPSO) to predict daily and total yields in solar power plants. Using data from two solar power plants over 34 days, the study enhances ANN predictions for solar power production. Results show PSO-optimized ANN achieved R-squared values between 72% and 88%, while WIPSO-optimized ANN achieved R-squared values between 68% and 88%, indicating significant accuracy.

## Introduction
Advancements in predictive analytics are crucial for optimizing solar power production. This study focuses on improving prediction accuracy of daily and periodic solar power yields by optimizing an ANN with PSO and WIPSO techniques. These methods address the nonlinear dynamics of solar power generation, leveraging extensive datasets from two solar power plants.

## Literature Review
Solar power plants convert sunlight into electricity using photovoltaic panels and inverters. Reliable performance depends on various environmental factors, and accurate yield prediction is essential for efficient management. This research integrates PSO and WIPSO with ANN to enhance forecasting accuracy.

## Data Collection and Preprocessing
### Dataset Description
The dataset, available on [Kaggle](https://www.kaggle.com/datasets/anikannal/solar-power-generation-data), was collected from two solar power plants in India over a 34-day period. It includes:
- **Power Generation Data**: Gathered at the inverter level, with multiple lines of solar panels attached to each inverter.
- **Sensor Readings Data**: Collected at a plant level from a single array of optimally placed sensors.

### Preprocessing Steps
- **Handling Missing Values**: Missing timestamps filled with zeros, and daytime missing entries reviewed and filled or removed.
- **Standardizing Data**: Daily yield standardized to zero when AC power is zero, and anomalies filtered out.
- **Feature Engineering**: Generated new features from sensor data, including cubic and quadratic terms of irradiance and ambient temperature.

### Results
- Memory footprint reduction for power production data: up to 78.19%.
- Reduction in missing entries for power production data: up to 34.38%.

## Methodology
### ANN Architecture
ANNs consist of input, hidden, and output layers. We used standard activation functions and adjusted weights and biases during training.

### Particle Swarm Optimization (PSO)
PSO is inspired by bird flocking behavior, optimizing solutions by updating velocities and positions. WIPSO improves PSO by dynamically adjusting inertia weight.

### Integration with ANN
PSO and WIPSO optimize ANN weights and biases to enhance model performance, balancing training accuracy and generalization.

## Experimental Setup
### Data Splitting
Data was split into training (80%) and testing (20%) sets.

### Performance Metrics
- **RMSE**: Measures average prediction error.
- **R-squared (R²)**: Indicates the proportion of variance predictable from independent variables.

## Results and Discussion
### Daily Yield
PSO and WIPSO-optimized ANN models closely followed actual values, showing effective predictions.

### Total Yield
Both models demonstrated strong performance in predicting cumulative energy production.

### Comparison
- **PSO**: RMSE between 115-181, R-squared between 72%-88%.
- **WIPSO**: RMSE between 116-192, R-squared between 68%-88%.

### Analysis
PSO-optimized ANN performed slightly better in terms of accuracy, but WIPSO showed competitive performance.

## Conclusion and Future Work
### Summary
Both PSO and WIPSO-optimized ANN models achieved high prediction accuracy for solar power yields. These models enhance operational efficiency and strategic planning in solar energy management.

### Implications
Accurate predictions improve energy management, reduce wastage, and aid in strategic planning. The models also support maintenance forecasting and resource optimization.

### Future Work
Future research could explore additional optimization algorithms, real-time predictive models, and integration with IoT devices for enhanced monitoring and decision-making.

## Code and Documentation
The code and its full documentation are provided in the `main.ipynb` notebook. This file includes detailed explanations of the methodology, results, and outputs. The approach and code were developed with reference to a Kaggle notebook: [Solar Power Plant Time Series Analysis](https://www.kaggle.com/code/elbiopea/solar-power-plant-time-series-analysis-v5-01-22).

Additionally, a detailed documentation of the work, including results, plots, and mathematical formulas, is available in the `full documentation.pdf` file.

## Contact
For further information, please contact maryamesh1911@gmail.com.
