# water stress proj

This project will be inspecting the effects of water stress found from remote sensing data.


> 1. Indentifying points of interest using change point detection
> 2. Use Casual Impact to measure the effect of a piont of interest
> 3. Applying the first two point to forcasts to aid preventative measures

![Image of Proj](https://github.com/jzyee/water_stress_proj/blob/master/images/overall_graph.png)

File descriptions:



 
 filename     |  description
 -------------|------------------------------------------------------------------------------------
 [sementation1.ipynb](https://github.com/jzyee/water_stress_proj/blob/master/segmentation1.ipynb) |  Creating the synthetic dataset                                             
   ---           |  Benchtesting the algorithms on the synthetic dataset
[all_in_one___periodic_wave.ipynb](https://github.com/jzyee/water_stress_proj/blob/master/all_in_one___periodic_wave.ipynb) | an example on how to use the classes made in this repo to benchmark the chang point algorithms on the datasets
r_files folder | contains all the necessary files to run the R environment to do the checks for BFAST and BEAST on the synthetic dataset

# requirements

cpdetect: https://github.com/choderalab/cpdetect
ruptures: https://centre-borelli.github.io/ruptures-docs/
casualimpact: https://github.com/dafiti/causalimpact

# References
* Ensign DL and Pande VS. Bayesian Detection of Intensity Changes in Single Molecule and Molecular Dynamics Trajectories. J. Phys. Chem B 114:280 (2010)
* C. Truong, L. Oudre, and N. Vayatis. Selective review of offline change point detection methods. Signal Processing, 167:107299, 2020.

