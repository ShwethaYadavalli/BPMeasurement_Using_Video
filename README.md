# Non-Invasive Blood Pressure Measurement Using Video Analysis
This project demonstrates a non-invasive method to estimate blood pressure (BP) using video analysis. The approach utilizes a video feed to capture the Photoplethysmogram (PPG) signal from a selected region of interest (e.g., the forehead) and applies machine learning techniques to predict blood pressure.

## Overview
The project captures a video feed, extracts the PPG signal from a specific region of interest, and uses the signal to predict blood pressure. The process involves the following steps:

**Capture Video**: Load a pre-recorded video or use a live camera feed.

**PPG Signal Extraction**: Identify a region of interest (ROI) in the video (e.g., forehead) and calculate the mean intensity of the ROI to derive the PPG signal.

**Signal Processing**: Process the PPG signal using techniques like peak detection and compute Pulse Transit Time (PTT).

**BP Prediction**: Train a machine learning model (Random Forest) using the extracted PTT features and predict BP values.

**Evaluation and Visualization**: Evaluate the model performance using metrics like Mean Squared Error (MSE) and R-squared (R²) and visualize the results.

## Requirements
1. Python 3.x

2. OpenCV

3. NumPy

4. SciPy

5. scikit-learn

6. Matplotlib

## Model Evaluation
The model is evaluated using the following metrics:

**Mean Squared Error (MSE)**: Measures the average squared difference between the actual and predicted BP values. Lower MSE indicates better model performance.

**R-squared (R²)**: Indicates the proportion of variance in the dependent variable (actual BP) that is predictable from the independent variable (features). R² values closer to 1 indicate better model performance.

## Visualization
The project includes the following visualizations:

**Actual vs Predicted BP Plot**: A scatter plot comparing actual BP values to predicted ones.

**PPG Signal with Detected Peaks**: A plot showing the PPG signal over time, with detected peaks highlighted.

**Feature Importance**: A bar chart showing the importance of different features in the Random Forest model.

### Advanced Analysis

**Feature Importance**: If using a RandomForestRegressor, you can explore the feature importance to understand which features contribute most to BP prediction.

**Signal Preprocessing**: Additional signal processing techniques like Butterworth filtering, detrending, etc., can be applied to enhance the quality of the PPG signal.

## Future Work
1. Future enhancements to the project could include:

2. Incorporating real BP measurement data to train the model.

3. Testing the approach with live video feeds for real-time BP monitoring.

4. Implementing advanced signal processing techniques to improve PPG signal quality.

5. Extending the model to consider additional physiological signals.
