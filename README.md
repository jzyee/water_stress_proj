# water stress proj

This project will be inspecting the effects of water stress found from remote sensing data.


> 1. Indentifying points of interest using change point detection
> 2. Use Casual Impact to measure the effect of a piont of interest
> 3. Applying the first two point to forcasts to aid preventative measures

![Image of Proj](https://github.com/jzyee/water_stress_proj/blob/master/images/overall_graph.png)



# How to Use

## 1. Load and normalize data

input data should be monthly resampled dataframe with NDVI,SPEI and predictive/correlating variables to help the forecasting
![loading](https://github.com/jzyee/water_stress_proj/blob/master/images/1.PNG)

## 2. Train model
> ![train](https://github.com/jzyee/water_stress_proj/blob/master/images/2.PNG)

## 3. add forecasted data to original data
![3](https://github.com/jzyee/water_stress_proj/blob/master/images/3.PNG)

## 4. init bench testing
![4](https://github.com/jzyee/water_stress_proj/blob/master/images/4.PNG)

## 5. run benchtesting
![6](https://github.com/jzyee/water_stress_proj/blob/master/images/6.PNG)

## 6. calculate casual impact for changepoints
first casual impact from dataframe is shown
![7](https://github.com/jzyee/water_stress_proj/blob/master/images/7.PNG)


File descriptions:



 
 filename     |  description
 -------------|------------------------------------------------------------------------------------
 [segmentation1.ipynb](https://github.com/jzyee/water_stress_proj/blob/master/segmentation1.ipynb) |  Creating the synthetic dataset                                             
   ---           |  Benchtesting the algorithms on the synthetic dataset
   [segmentation2.ipynb](https://github.com/jzyee/water_stress_proj/blob/master/segmentation2.ipynb) | prototyping on the real NDVI dataset
   ---           | check witch changepoints like in the drought-linked pointer years
[all_in_one___periodic_wave.ipynb](https://github.com/jzyee/water_stress_proj/blob/master/all_in_one___periodic_wave.ipynb) | an example on how to use the classes made in this repo to benchmark the change point algorithms on the datasets
[benchmark.py](https://github.com/jzyee/water_stress_proj/blob/master/benchmark.py) | benchmarking class to run the benchmarks
[helper.py](https://github.com/jzyee/water_stress_proj/blob/master/helper.py)| file containing helper functions
[lstm_model.py](https://github.com/jzyee/water_stress_proj/blob/master/lstm_model.py)|file containing the model to facilitate forecasting
r_files folder | contains all the necessary files to run the R environment to do the checks for BFAST and BEAST on the synthetic dataset

# requirements

* cpdetect: https://github.com/jzyee/cpdetect
* ruptures: https://centre-borelli.github.io/ruptures-docs/
* casualimpact: https://github.com/dafiti/causalimpact

# References
* Ensign DL and Pande VS. Bayesian Detection of Intensity Changes in Single Molecule and Molecular Dynamics Trajectories. J. Phys. Chem B 114:280 (2010)
* C. Truong, L. Oudre, and N. Vayatis. Selective review of offline change point detection methods. Signal Processing, 167:107299, 2020.

