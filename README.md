# PCR-Chemistry
Principal Component Regression for chemical spectroscopy multivariate calibration. Written in Python with TKinter-based GUI. 

It reads the spectral CSV data, performs Savitzky–Golay preprocessing, performs PCR multivariate calibration, and outputs predicted concentrations as a CSV file. 

To run the PCR.py file you will need the following dependencies: 
<ul>
  <li>Pandas/li>
  <li>Numpy</li>
  <li>Matplotlib</li>
  <li>Scipy</li>
  <li>Scikit-learn</li>
  <li>Customtkinter</li>
</ul> 

After running PCR.py, you will need to enter four .csv files:
<ul>
  <li>Spectral data (absorbance) of the standards (training)</li>
  <li>Wavelength or wavenumber values the spectral data were colected</li>
  <li>Known concentrations of the standards (training)</li>
  <li>Spectral data (absorbance) of the sample</li>
</ul> 

The data in these files must be in the correct format as follows:





