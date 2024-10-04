# Biodefense Analytics Project: GPU-Accelerated Epidemic Response

Welcome to the Biodefense Analytics Project repository. This project was part of a course aimed at harnessing the power of GPU-accelerated computing using RAPIDS and other powerful data science tools to tackle the challenges posed by large-scale epidemic simulations.

## Overview

In this project, I worked on a simulation modeled on the spread of a virulent virus in the UK. Over several weeks, the course took me through various stages of epidemic response, from containment efforts to crisis management. Each stage demanded sophisticated data analytics, leveraging millions of rows of data and Nvidia’s GPU-accelerated ecosystem to derive insights and inform action.

## Project Highlights

- **Dataset**: A simulated epidemic dataset containing millions of rows (~58 mil) of geographical, demographic, and healthcare data.
- **Tools**: Nvidia RAPIDS ecosystem tools such as cuDF, cuML, Dask, cuGraph, cyPy, Apache Arrow, running on a multi-GPU environment.

### Key Skills Developed

- Managing large datasets with cuDF.
- Performing parallelized machine learning with cuML.
- Distributed computing with Dask to handle the massive data load.
- Graph analytics using cuGraph to understand virus spread.
- Working with in-memory columnar data using Apache Arrow.
- Utilizing cuXFilter for interactive visualization and data exploration.

## Weekly Breakdown

### Week 1: Containment Strategy

- **Challenge**: A virus is rapidly spreading, and we needed to identify dense geographic clusters of infected individuals.
- **Objective**: Contain the virus before it spreads further.
- **Tools**: cuDF for managing millions of rows of geographic and infection data, and cuGraph for analyzing clusters.
- **Outcome**: Discovered several high-density clusters using DBSCAN, allowing authorities to focus containment efforts.

### Week 2: Logistics for Response

- **Challenge**: With the virus out of control, we shifted to logistical planning to manage medical resources.
- **Objective**: Match infected individuals to their nearest medical facilities to estimate the capacity requirements.
- **Tools**: Dask for distributed computing across the dataset, cuML for regression analysis to predict hospital demand.
- **Outcome**: Efficiently matched individuals to hospitals using KNN, helping prepare the healthcare system for an overwhelming influx of patients.

### Week 3: Crisis Management and Risk Assessment

- **Challenge**: The epidemic was reaching critical levels, infecting 1 in every 200 people. We needed to understand which populations were most at risk.
- **Objective**: Use demographic and employment data to identify high-risk groups.
- **Tools**: cuDF and cuML for demographic analysis, cyPy for Python-driven modeling.
- **Outcome**: Identified key risk factors using cuDG, cuXFilter, allowing authorities to target interventions toward the most vulnerable populations.

## Technologies Used

- **RAPIDS Ecosystem**
  - **cuDF**: Used to manipulate and clean large datasets with a focus on GPU acceleration.
  - **cuML**: Machine learning tasks like clustering and regression were executed using cuML’s highly optimized algorithms.
  - **cuGraph**: Graph analytics to analyze geographic clusters of infected individuals.
  - **cuXFilter**: Utilized for interactive visualization and data exploration, enabling real-time insights into the epidemic spread.
  - **Dask**: Leveraged for parallel and distributed computing, allowing us to handle the millions of data points efficiently.
  - **Apache Arrow**: Ensured fast in-memory data transfers between components of the RAPIDS ecosystem and other tools.

- **GPU Environment**
  - This project was executed on Nvidia’s multi-GPU infrastructure, using:
    - Nvidia 4 Tesla T4 GPUs for high-performance computing.
  
Nvidia’s RAPIDS tools allowed me to perform complex data transformations and machine learning in a fraction of the time it would have taken with a CPU-based approach.

## What I Learned

- **Leveraging GPU Acceleration**: I learned how to use GPUs to accelerate data science tasks, from data manipulation to machine learning, leading to significant performance gains.
- **Scaling with Dask**: By distributing computations, I managed millions of rows efficiently, ensuring the project could scale.
- **Graph Analytics with cuGraph**: Understanding the virus spread through geographic graph clusters was a crucial skill developed.
- **Real-World Data Analysis**: The simulation was based on real-world research into Ebola virus risk factors, giving me hands-on experience with pandemic modeling.


Assessment Project as part of Nvidia's Instructor Led Course at University of Florida: GPU-Accelerated Data Manipulation


