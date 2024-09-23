# Traveltime Approximation Methods in Seismic Data Processing

## Project Overview

This project focuses on computing the **traveltime** of seismic waves through various **1D subsurface velocity** and **thickness models** using ray theory concepts. It addresses the hyperbolic relationship between **time** and **offset** in seismic data. Several **approximation methods** are applied to improve the accuracy of traveltime computations, particularly at **far offsets**. The ultimate goal is to identify suitable methods to reduce **NMO (Normal Moveout)** distortions in seismic processing.

$$
T(x) = \sqrt{T_0^2 + \left( \frac{x}{V_{rms}} \right)^2 }
$$

## Key Features

- **1D Velocity and Thickness Models:**  
  The notebook operates on different subsurface models, characterized by their **velocity** and **thickness** properties.

- **Hyperbolic Traveltime Relation:**  
  The time-offset relationship in seismic data follows a hyperbolic curve:

  $$
  T(x) = \sqrt{T_0^2 + \left( \frac{x}{V_{rms}} \right)^2 }
  $$

- **Approximation Methods:**
    1. **Taylor Approximation:**  
       Applied up to the **nth degree** to approximate the traveltime relation.
    2. **Pade Approximation:**  
       **nth-order Pade approximation** is used for higher accuracy at **far offsets**.
    3. **Ghosh Kumar Approximation:**  
       A specialized method applied to improve the traveltime approximation.
    4. **Hybrid Approximation:**  
       A combination of the **Taylor** and **Ghosh Kumar** methods to achieve optimal results.

- **RMS Error Calculation:**  
  The notebook computes the **root-mean-square (RMS) error** for each approximation method, assessing its accuracy and effectiveness in reducing **NMO distortions** at far offsets.

## Requirements

To run this notebook, install the following Python libraries:

```bash
pip install numpy scipy matplotlib plotly tqdm
