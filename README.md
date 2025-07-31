# PCR-Chemistry

Principal Component Regression for chemical spectroscopy multivariate calibration. Written in Python with TKinter-based GUI. 

This tool reads spectral CSV data, applies **Savitzky–Golay preprocessing**, performs **PCR calibration**, and outputs the **predicted concentrations** as a CSV file. 

# What is PCR

The Principal Components Regression (PCR) is a combination of Ordinary Least Squares Regression (OLS) with **Principal Components Analysis** (PCA). PCA reduces the dimensionality of the spectral data while reducing the **multicollinearity**, this helps the model to differentiate the values of the independent variables. Then, OLS models the linear relationship between the variables. As a result, PCR provides a multivariate linear model that is **more robust** than the classical calibration method. 

In that process, the dimensionality of the spectral data is reduced to **principal components**, which the optimum number is determined by **cross-validation**. 

***

To run the `PCR.py` file make sure the following dependencies are installed: 
<ul>
  <li>Pandas</li>
  <li>Numpy</li>
  <li>Matplotlib</li>
  <li>Scipy</li>
  <li>Scikit-learn</li>
  <li>Tkinter</li>
  <li>Customtkinter</li>
</ul> 

After running `PCR.py`, the GUI will prompt you to upload four `.csv` files:
<ul>
  <li>Spectral data (absorbance) of the standards (training)</li>
  <li>Wavelength or wavenumber values the spectral data were colected</li>
  <li>Known concentrations of the standards (training)</li>
  <li>Spectral data (absorbance) of the sample</li>
</ul> 

Each file must follow a specific format:

![image_alt](https://github.com/JLFernandes11/PCR-Chemistry/blob/7e6930f361069db558a2df97395400513e6a7eee/Screenshot.png)

You can test the application using:
<ul>
  <li>standards_spectral.csv</li>
  <li>wavelength.csv</li>
  <li>standard_concentrations.csv</li>
  <li>sample_simulation.csv</li>
</ul> 

Output:
<ul>
  <li>Preprocessing and calibration plots will be shown.</li>
  <li>Model performance metrics will be shown.</li>
  <li>Final predicted concentrations are saved as "predicted_concentrations_pcr.csv".</li>
</ul> 

