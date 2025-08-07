# Sen2Clean
Sen2Clean remove cloud and clean time series of vegetation index from Sentinel-2, focusing on:

 - Cloud masking using the Scene Classification Layer (SCL)
 - Temporal compositing (e.g. 16-day maximum VI)
 - Noise reduction by detecting and removing unrealistic noisy local minima (often caused by undetected clouds)

# Main Features
- Masks clouds using SCL classes and a configurable valid pixel threshold
- Generates maximum-value composites over fixed intervals (default: 16 days)
- Removes residual noise using local minima filtering

# Requirements
xarray
numpy
pandas

Install using:

bash pip install xarray numpy pandas


# Licence
Released under the MIT Licence.
