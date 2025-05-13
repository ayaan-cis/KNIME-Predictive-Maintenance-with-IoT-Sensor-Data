# KNIME Predictive Maintenance with IoT Sensor Data

Image of workflow will go here.

## Project Overview

This repository contains a comprehensive predictive maintenance system built with the KNIME Analytics Platform. The system uses IoT sensor data from aircraft engines to predict potential failures before they occur, demonstrating both technical data science expertise and practical business value.

### Business Value

Predictive maintenance offers significant advantages over traditional reactive or scheduled maintenance approaches:

- **Cost Reduction**: Minimize downtime and avoid catastrophic failures
- **Extended Equipment Life**: Optimize maintenance scheduling
- **Improved Safety**: Prevent failures in critical operations
- **Resource Optimization**: Allocate maintenance resources efficiently

## Dataset

This project utilizes the NASA Turbofan Engine Degradation Simulation Dataset from the [NASA Prognostics Data Repository](https://www.nasa.gov/content/prognostics-center-of-excellence-data-set-repository/). The dataset includes:

- Multiple sensor readings from aircraft engines
- Run-to-failure data for training
- Test data for prediction validation
- Ground truth Remaining Useful Life (RUL) values

## Methodology

The project follows a structured data science approach:

1. **Data Preprocessing**
   - Handling missing values and outliers
   - Feature scaling and normalization
   - Time series alignment

2. **Exploratory Data Analysis**
   - Sensor correlation analysis
   - Degradation pattern visualization
   - Anomaly identification

3. **Feature Engineering**
   - Time-based feature extraction
   - Sliding window aggregations
   - Sensor trend calculations
   - RUL (Remaining Useful Life) target creation

4. **Model Development**
   - Random Forest for RUL prediction
   - Gradient Boosting for failure classification
   - Isolation Forest for anomaly detection
   - Model ensemble techniques

5. **Evaluation & Optimization**
   - Cross-validation approaches
   - Hyperparameter optimization
   - Performance metric analysis

## KNIME Workflow Structure

![Workflow Overview](https://your-repo-url/assets/workflow-overview.png)

The KNIME workflow is organized into logical components:

- 📊 **Data Ingestion**: Reading and initial processing of sensor data
- 🧹 **Preprocessing**: Cleaning, normalization, and preparation
- 🔍 **EDA**: Interactive visualizations and statistical analysis
- ⚙️ **Feature Engineering**: Creating predictive variables
- 🤖 **Modeling**: Training and tuning predictive models
- 📈 **Evaluation**: Assessing model performance
- 📑 **Reporting**: Generating interactive visualizations and findings

## Results

The predictive maintenance system achieves:

- **XX%** accuracy in predicting failures within a 20-cycle window
- **XX%** reduction in false positives compared to threshold-based approaches
- Estimated cost savings of **$XXX,XXX** per year in a typical manufacturing setting

## Interactive Visualizations

This repository includes interactive visualizations created with KNIME's JavaScript views:

Implementations of visualizations will go here.

## How to Use This Project

### Prerequisites

- [KNIME Analytics Platform](https://www.knime.com/downloads) (version 4.7.0 or higher)
- NASA Turbofan Engine Degradation Simulation Dataset

### Installation

1. Clone this repository
2. Download the dataset from the NASA Prognostics Repository
3. Open KNIME and import the workflow file
4. Update file paths in the File Reader nodes
5. Execute the workflow

## Technical Challenges and Solutions

During development, several technical challenges were addressed:

1. **Time Series Alignment**: Engines start with different initial wear conditions
   - Solution: Normalized cycle count and created relative measures

2. **Feature Selection**: Identifying most predictive sensors
   - Solution: Implemented recursive feature elimination within KNIME

3. **Imbalanced Data**: Limited failure examples compared to normal operation
   - Solution: Applied synthetic minority oversampling techniques

## Future Improvements

Potential enhancements to this project include:

- Integration with real-time data streams
- Deployment as a KNIME WebPortal for interactive use
- Addition of deep learning models (LSTM/Transformer)
- Expansion to multi-class fault classification


## Acknowledgments

- NASA Prognostics Data Repository for the dataset
- KNIME Community for node examples and inspiration

---

© 2025 [Ayaan Syed] | Licensed under MIT License
