**Project Overview**
This project is focused on computing the traveltime of seismic waves through various 1D subsurface velocity and thickness models using ray theory concepts. It aims to address the hyperbolic relationship between time and offset in seismic data and applies several approximation methods to improve the accuracy of traveltime computations, particularly at far offsets. The ultimate goal is to identify suitable methods to reduce NMO (Normal Moveout) distortions in seismic processing.

**Key Features**
**1D Velocity and Thickness Models:** The notebook operates on different subsurface models, characterized by their velocity and thickness properties.
**Hyperbolic Traveltime Relation**: The notebook deals with the time-offset relationship, which is inherently hyperbolic in seismic data.
**Approximation Methods:**
Taylor Approximation: Applied up to the nth degree to approximate the traveltime relation.
Pade Approximation: nth-order Pade approximation for higher accuracy at far offsets.
Ghosh Kumar Approximation: Another method applied to improve the traveltime approximation.
Hybrid Approximation: A combination of the Taylor and Ghosh Kumar methods to achieve optimal results.
RMS Error Calculation: The notebook computes the root-mean-square (RMS) error for each approximation method to evaluate its accuracy and effectiveness in reducing NMO distortions.
**Requirements**
To run this notebook, you will need the following Python libraries:

numpy: For numerical computations.
scipy: For scientific computing, including linear algebra and mathematical functions.
matplotlib: For generating visual plots of the traveltime approximations.
plotly: For interactive visualization of the results.
decimal: For handling high-precision floating-point arithmetic.
tqdm: For progress bars to track the computation process.
