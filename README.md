# DOG
A Jython script for [Fiji/ImageJ](https://github.com/fiji) to perform [Difference of Gaussians](http://en.wikipedia.org/wiki/Difference_of_Gaussians) on fluorescent stack and plot the result.

This script will open a single channel fluorescent stack, perform the Difference of Gaussians and then plot all found points with the orthoslice view

## Parameters available :
- cellDiameter : select the cell/nucleus diameter (in unit of the Image Stack)
- minPeak : min intensity for a peak to be considered
- plotType : plot Points, Icospheres or limit to the first 3495 points due to some slowdown with Icospheres
- cellIcosophere : size of the point/icosphere use to visualize each detected point.

## TODO: 
- Apply 3D Watershed segmentation using the detected points has a seed (see [3D Watershed plugin](http://imagejdocu.tudor.lu/doku.php?id=plugin:segmentation:3d_spots_segmentation:start#d_watershed) )
- Allow multiple channels in the stack
- Add a dialog for the parameters
- Add interface to measure nucleus/cell parameters
