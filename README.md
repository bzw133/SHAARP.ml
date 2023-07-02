![GitHub release version](https://img.shields.io/github/v/release/bzw133/SHAARP.ml?color=%2350C878&include_prereleases)
![License](https://img.shields.io/github/license/Rui-Zu/SHAARP)
![GitHub Size](https://img.shields.io/github/repo-size/bzw133/SHAARP.ml)
[![HitCount](https://hits.dwyl.com/Rui-Zu/SHAARP.svg?style=flat-square)](http://hits.dwyl.com/bzw133/SHAARP.ml)
[![HitCount](https://hits.dwyl.com/Rui-Zu/SHAARP.svg?style=flat-square&show=unique)](http://hits.dwyl.com/bzw133/SHAARP.ml)

# Welcome to ♯SHAARP._ml_ 

**♯SHAARP**._ml_ is an open-source package for modeling reflected and transmitted optical second harmonic generation (SHG) of slab and multilayer structures of nonlinear optical materials. 

This package builds upon a general approach to solve the Maxwell equations under proper boundary conditions to obtain the SHG responses of various materials systems. The package is designed to handle **arbitrary number of layers, number of SHG active media, crystal symmetry, crystal orientations, complex refractive indices, and polarized incident lights**. The two most common SHG characterization approaches, Maker fringes and polarimetry, are integrated into the package. 

**♯SHAARP**._ml_ is also a successor of the **♯SHAARP**._si_, which was designed for modeling the reflected SHG responses of a single-interface system.  

# Features and Applications 

**♯SHAARP**._ml_ exhibits unique features for modeling the SHG responses with flexibility, high-fidelity, high accuracy, high efficiency, user-friendliness, and extensibility.   

Key features of **♯SHAARP**._ml_ include:  
- Flexibility in defining the multilayer structure, materials properties, incident lights, and assumptions for the SHG polarization   
- High-fidelity as verified by benchmarking with established analytical theories in literature and experimental validation of more than eight material systems  
- High accuracy as the solutions are all semi-analytical with minimal numerical approximations  
- High efficiency as it typically takes a few seconds calculation time for single incidence of multilayers (tested with heterostructure consisting of eight different SHG active layers) 
- User-friendliness with well-designed GUI and documentations, more than ten preset cases studies and tutorials videos
- Extensibility as it is programmable with modularized functions beside the GUI   

**♯SHAARP**._ml_ is designed for two types of studies:  
1. To numerically simulate SHG responses of nonlinear optical materials and  heterostructures  
2. To obtain analytical expressions of SHG responses and fit experimental measurements to determine the nonlinear optical properties of materials 

# Quickstart 

## Installation 

- ♯SHAARP._ml_ is written as a notebook using Wolfram Language and the access to _Mathematica®_ or *Wolfram Player* is required to run **♯SHAARP**._ml_ on PC/Mac. Please refer to the [Installing Mathematica](https://reference.wolfram.com/language/tutorial/InstallingMathematica.html).
- Download SHAARP.ml_V\#\.zip in the latest release from [here](https://github.com/bzw133/SHAARP.ml).
- Unzip the file and you will obtain two _Mathematica®_ notebooks: 
	- SHAARP.ml.nb
	- setup.nb

## Run the SHAARP.*ml* notebook 
- Open SHAARP.ml.nb 
- Make sure that Dynamic Evaluation is enabled, evaluate the notebook by clicking `Evaluation > Evaluate Notebook` from the menu bar. Note that this process clears all the definitions from the other currently open notebooks. 
- You will get the welcome page as: 
  ![[readme-welcome.png]]

## Run the default case study 
- There is a default single slab system (1 $\mu m$-thick Z-cut LiNbO3 slab, incident wavelength = 1.064 $\mu m$) for quick test calculation.
- To visualize the setup of the system, click `Set Material Properties` in the `Functionality` subpanel, and then click `Update`. You will get: 
  ![[LNO-setup.png]]
- To simulation the SHG response of the system, click `SHG Simulation` in the `Functionality` subpanel, and then click `Update`. You will get: 
  ![[LNO-sim.png]]
- To obtain the partial analytical expressions of the SHG responses, click `Partial Analytical Expressions`, and then click `Update`. You will get: 
  ![[readme-analytic.png]]
- For advanced usage such as Maker fringes simulation, please refer to the  [documentation](https://shaarpml.readthedocs.io/en/latest/ ). 


# Gallery
- Arbitrary number of layers with a mixture of linear and SHG active materials 
  ![[8-layer-structure.png]]
- Full SHG simulation results of a 100 $\mu m$-thick Z-cut LiNbO3 slab (with JK assumptions), including  
	- Wave propagation plots
	- Reflectance and transmittance (Fresnel coefficients) of linear waves 
	- Maker fringes of SHG waves
![[LNO-full-sim.png]]
- 3D schematics of polarizer and analyzer and ellipticity of waves 
  ![[pol.png]]
- Partial analytical solutions of a 300 $\mu m$-thick Z-cut Quartz slab
	- with slab thickness (h1) and SHG d33 and d14 coefficients as unknown variables
	- full multiple reflection assumption
![[quartz-full-analytic.png]]

# To learn more

- Please refer to the [documentation](https://shaarpml.readthedocs.io/en/latest/ ) to learn more advanced topics and tips about **♯SHAARP**._ml_. 
- For theoretical detail and experimental validation of **♯SHAARP**._ml_ approach, please refer to our publications: 
	- **Zu, R., Wang, B., He, J. et al. Analytical and numerical modeling of optical second harmonic generation in anisotropic crystals using ♯SHAARP package. npj Comput Mater 8, 246 (2022). [https://doi.org/10.1038/s41524-022-00930-4](https://doi.org/10.1038/s41524-022-00930-4)**
	- **Zu, R., Wang, B., He, J. et al. Optical Second Harmonic Generation in Anisotropic Multilayers with Complete Multireflection Analysis** **of Linear and Nonlinear Waves using ♯SHAARP._ml_ Package, (2023), arxiv.**

## Links 
- Code repository of **♯SHAARP**._ml_: https://github.com/bzw133/SHAARP.ml
- Documentation of **♯SHAARP**._ml_: https://shaarpml.readthedocs.io/en/latest/ 
- Tutorial videos **♯SHAARP**._ml_: https://youtu.be/YiKRm6i7kNs
- The **♯SHAARP** package for single interface (**♯SHAARP**._si_): 
	- Code repository: https://github.com/Rui-Zu/SHAARP
	- Documentation: https://shaarp.readthedocs.io/en/latest/
	- Tutorial videos: https://www.youtube.com/watch?v=fr0RirVHXVc

## Referencing
If you've used **♯SHAARP**._ml_ in any publication of you, please cite the references:
1. **Zu, R., Wang, B., He, J. et al. Optical Second Harmonic Generation in Anisotropic Multilayers with Complete Multireflection Analysis** **of Linear and Nonlinear Waves using ♯SHAARP._ml_ Package, (2023), arxiv.**
2. **Zu, R., Wang, B., He, J. et al. Analytical and numerical modeling of optical second harmonic generation in anisotropic crystals using ♯SHAARP package. npj Comput Mater 8, 246 (2022). [https://doi.org/10.1038/s41524-022-00930-4](https://doi.org/10.1038/s41524-022-00930-4)**

## Acknowledgement
This development of the software was supported as part of the Computational Materials Sciences Program funded by the U.S. Department of Energy, Office of Science, Basic Energy Sciences, under Award No. DE-SC0020145.
