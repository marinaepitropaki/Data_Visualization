# Data_Visualization
This repository contains valuable tools for visualizing data from astronomical images of massive data sets.

## Calibration_data_visualization script
* Loads data (biases, darks, flats) from specific path
* Calculates the median and the average of the each file
* Calculates the median and the average of the master file
* Calculates the average of the averages
* Visualizes the data
* Flattens the original data
* Visualizes each file in a block of histograms
* Visualizes the master file in a histogram
* Loads at least three files random from the path and visualize them in the same histogram with the master file
## Photometry_one_star script
* Loads aligned images of an object
* Finds the center of the object using DS9
* Crops the area of the file with the object to examine
* Plots the data for horizontal and vertical axes
* Implements gauss fitting
* Visualizes the object in a plot of pixels
* Finds the maximum point of the curve
* Crops an even smaller area that contains only the object closely, using the gauss parameters
* Plots this smaller area
* Creates a function that masks the second crop in order to calculate the background
* Creates a list with  data from the second crop 
* Removes the background of this data
* Plots the object data with and without background for comparison

## Photometry_three_stars script
* Loads aligned images of an object
* Finds the center of a object and two more of similar intensity for comparison using DS9
* For those three objects in all the files in total:
* Crops the area of the file with the object to examine
* Plots the data for horizontal and vertical axes
* Implements gauss fitting
* Visualizes the object in a plot of pixels
* Finds the maximum point of the curve
* Crops an even smaller area that contains only the object closely, using the gauss parameters
* Plots this smaller area
* Creates a function that masks the second crop in order to calculate the background
* Creates a list with data from the second crop 
* Removes the background of this data
* Saves the FWHM and x0 gauss parameters in CSV file
* Plots the Time-Intensity diagram for the 3 objects
* Plots the main object data with and without background for comparison
* Normalizes the objects and plot for comparison
* Creates CSV file that contains time and flux values for all the reduced from background objects (unnormalized)

