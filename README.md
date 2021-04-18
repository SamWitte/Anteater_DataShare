# Data output produced from code: Anteater (AxioN-phoTon convErsion in mAgneTosphERes). This was data generated for the use in arXiv: 

Details on Anteater (to be made public in near future):
~~~~~~~~~~~~~~~~~~~~
This code is intended to accurately compute the expected radio signal from axion-photon conversion in the magnetospheres of neutron stars. At the moment this is currently written for the Goldreich-Julien model, and assuming an axion phase space distribution consistent with a neutron star at rest relative to the dark matter halo. The primary code is written in Julia, and the plots are generated partially with Julia and partially with python. 


** Important, the files must be downloaded Zenodo, with doi link: 10.5281/zenodo.4604619  (https://zenodo.org/record/4604619#.YHxdYxSA52R)
These files should be put in src/results directory.


 The format of the files is as follows:

- src:
	- RayTracer.jl: This is the main file, which samples the axion phase space at the conversion surface, generates photon trajectories (properly weighted by their contribution to the rate), computes the energy broadening induced from both the asymptotic distribution and the plasma interactions, computes the absorption probability from the cyclotron resonance, and outputs files containing information on the photons and their trajectories (files are output to (/src/results directory).
	- Gen_Samples.jl: This file is a wrapper for the RayTracer.jl. Input the parameters you wish to run, and this file will pass all relevant info to the ray tracer.

- notebook_examples
	- There are two notebooks, one which generates plots from the paper which were made in python, the other which generates plots from the paper made in Julia.
	- One of the plots in the python notebook requires unzipping the Sample_Trajs directory.
	- We also include a gif (in directory Gif). This can be run on a Mac by highlighting the file with your cursor, and pressing simultaneously command + y



Questions/comments/concerns about the code can be directed to Sam Witte at the following email address: s.j.witte@uva.nl 
