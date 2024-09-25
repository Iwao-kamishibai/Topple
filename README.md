# Topple
Topple is a Shiny app for geological analysis of rock block dimensions and statistical properties.



The Topple app is an interactive Shiny web application designed for geological and geotechnical analysis of rock block dimensions and geometries, specifically to assess the risk of rockfall events. It allows users to upload datasets containing measurements of rock blocks—specifically, the lengths of the blocks along the x, y, and z axes. The app performs comprehensive statistical analyses on these measurements to help users understand the distribution and characteristics of the rock blocks in their dataset.

Key Features:

Data Upload and Processing:

Users can upload a CSV file containing their block dimension data. The app calculates additional variables such as block volume and axial ratios (y/x and z/y).

Statistical Analysis:

Provides main statistical values including measures of central tendency (mean, median) and dispersion (standard deviation, variance, interquartile range). Calculates skewness and kurtosis to assess the empirical distribution form of the block volumes.

Visualization Tools:

Block Size Distribution Histogram: Displays the percentage of blocks within predefined volume classes. Helps in understanding the overall size distribution of the blocks. Cumulative Distribution Function (ECDF) Plot: Shows the cumulative distribution of the log-transformed block volumes. Allows users to identify specific percentiles, such as the mean, median, and a user-selected percentile (e.g., 95th percentile).

Axial Ratio Scatter Plot:

Plots y/x versus z/y ratios to categorize block shapes based on their geometry. Classifies blocks into quadrants (A, B, C, D) following the method of Franklin & Dussault (1989), indicating shapes like platy, cubic, prismatic, or rod-like.

Report Generation:

Enables users to generate comprehensive PDF and Word reports summarizing their analyses. Reports include data samples, statistical summaries, plots, and annotations highlighting key findings. Use Cases:

Interactive Analysis:

Users can adjust parameters like the percentile of interest and see immediate updates in the analysis and plots.

Comprehensive Reporting:

Automated report generation saves time and ensures consistency in documentation.

Data Preperation:

1.) Collect Data: Record three dimensions (x, y, z) for each rock block in meters.

2.) Ensure Measurements: Use decimal format (e.g., 0.3).

3.) Organize Data:

Nr.: Index starting from 1.
x: Longest dimension.
4.) Reorder Dimensions: Make sure x is the largest

5.) Save as CSV: Export the file as a CSV (e.g., block_data.csv).

6.) Upload: Upload the CSV to the Topple app and enjoy your statistical analysis..

Data Example:

Nr.	x	y	z
1	0.30	0.20	0.20
2	0.40	0.40	0.15
3	0.25	0.20	0.15
4	0.25	0.20	0.15
5	0.50	0.30	0.25
