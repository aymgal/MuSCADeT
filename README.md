========================================================
INSTALLATION: 
- Download and unzip the M2CAD.zip file
- Open the M2CAD folder
- Install the python package:
"python setup.py install"

========================================================
The results presented in Joseph et al. 2015 can be recovered by running the script provided in the "Example" folder. The scripts can be used to run our algorithm on other data. 

In M2CAD, open the Examples folder and execute:
"python Example_simple.py"

Inputs provided in the Simu_simple folder:
-Cube.fits (fits file with input images)
-Simu_A.fits (mixing matrix used to generate the simulations)

Results are written in the "Simu_simple" folder.
After the execution, one can find the following files in the Simu_simple folder:
-Blue_residuals.fits (fits RGBcube with result from subtraction of red source from original band images)
-Colour_residuals.fits (fits RGBcube with result from subtraction of red and blue sources from original band images)
-Red_residuals.fits (fits RGBcube with result from subtraction of blue source from original band images)
-Estimated_A.fits (mixing matrix as estimated from spectral PCA)
-Sources_100.fits (fits cube with sources extracted by M2CAD: the direct product of our algorithm)


All "Example_-.py" files can be used the same way. Each Simu_- folder contains the benchmark data or real images to be treated in the “Cube.fits” fits cube and the mixing coefficients used to generate the simulations in “Simu_A.fits”.
"Example_refsdal.py" runs the algorithm on the real images of MACS J1149+2223 and writes the results in Simu_Refsdal_big

Users may change the input parameters via the same files and are encouraged to use them for further applications.




