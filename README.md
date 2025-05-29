# spark-google-cluster-analysis
# Google Cluster Data Analysis with Apache Spark

## Overview

This project focuses on analyzing large-scale data using **Apache Spark** on the [Google Cluster Data 2011 dataset](https://github.com/google/cluster-data). The dataset captures 29 days of activity across a cluster of ~12,500 machines, offering real-world insight into resource utilization, task scheduling, and system behavior in large-scale distributed environments. This work was conducted as part of the **Large-Scale Data Management** course at Université Grenoble Alpes – Master M2 MOSIG.

## Project Goals

1. **Cluster Insight**: Analyze CPU capacity, job/task distribution, and system maintenance events across thousands of machines.
2. **Task Scheduling & Eviction**: Study eviction patterns and scheduling classes to uncover trends and inefficiencies in workload management.
3. **Resource Efficiency**: Evaluate alignment between requested and consumed resources using CPU/memory ratios.
4. **Predictive Modeling**: Train machine learning models to predict task evictions using Spark MLlib, Scikit-learn, and deep learning frameworks.
5. **Framework Comparison**: Compare the capabilities and performance of Spark vs Pandas, and traditional ML vs Neural Networks (TensorFlow, PyTorch).

## Dataset

The **Google Cluster Data 2011** dataset contains time-series logs of jobs, tasks, and machine resource usage over a 29-day period. Key components include:

- **Machine Events**: Track machine additions, removals, and maintenance.
- **Job & Task Events**: Contain metadata such as scheduling class, priority, and runtime events.
- **Task Usage**: Time-windowed CPU, memory, and disk I/O metrics for every task.
- **Attributes & Constraints**: Provide additional (often obfuscated) machine details.

📁 **Dataset Source**: [ClusterData2011_2 on GitHub](https://github.com/google/cluster-data)

## Features

- **Descriptive Analysis**:
  - Distribution of machine CPU capacities
  - Percentage of CPU lost to maintenance events
  - Jobs and tasks grouped by scheduling class
- **System Behavior Analysis**:
  - Eviction rates vs scheduling class
  - Task distribution across machines
  - Resource over-provisioning vs real usage
- **Custom Research Questions**:
  - Average resource usage by scheduling class
  - Predicting task eviction using ML
- **Framework & Performance Extensions**:
  - Spark vs Pandas runtime/memory comparison
  - AUC comparison across Spark MLlib, Scikit-learn, TensorFlow, and PyTorch
  - Feature importance ranking in eviction prediction

## Technologies Used

- **Apache Spark** (DataFrames + MLlib)
- **Python**
- **Pandas, Matplotlib, Seaborn**
- **Scikit-learn**
- **TensorFlow**
- **PyTorch**
- **Jupyter Notebooks**

## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/your-username/spark-google-cluster-analysis.git
    ```

2. **Navigate to the Project Directory**:
    ```bash
    cd spark-google-cluster-analysis
    ```

3. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the Notebook**:
    ```bash
    jupyter notebook Fares_Shehazi.ipynb
    ```

## Usage

The notebook walks through all steps:

1. **Loading and Parsing CSV Files** with Spark
2. **Data Cleaning and Preprocessing**
3. **Answering the 7 pre-defined analytical questions**
4. **Exploring 2 custom questions**:
   - Average resource usage by scheduling class
   - Task eviction prediction using ML
5. **Model Training & Comparison** using:
   - Spark MLlib
   - Scikit-learn
   - TensorFlow and PyTorch
6. **Visualizations**: Histograms, bar charts, heatmaps, ROC curves

## Repository Structure

