![GitHub release version](https://img.shields.io/github/v/release/Rui-Zu/SHAARP?color=%2350C878&include_prereleases)
![License](https://img.shields.io/github/license/Rui-Zu/SHAARP)
![GitHub Size](https://img.shields.io/github/repo-size/Rui-Zu/SHAARP)

# Welcome to ♯SHAARP._ml_ 
---
**♯SHAARP**._ml_ is an open-source package for modeling reflected and transmitted optical second harmonic generation (SHG) of a single-layer slab and multi-layer heterostructure of nonlinear optical materials. 

This package builds in the most general approach to both analytically and numerically solving the SHG response of various materials systems. The package is designed to handle **arbitrary number of layers, number of SHG active mediums, crystal symmetry, arbitrary orientation, complex refractive indices, and arbitrary polarization state of light** (e.g., linearly, circularly, elliptically polarized). The two most common SHG characterization approaches, Maker fringes and polarimetry, are integrated into the package. 

**♯SHAARP**._ml_ is also a successor of the **♯SHAARP**._si_, which was designed for modeling the reflected SHG responses for an single interface.  

# Features and Applications 
---

**♯SHAARP**._ml_ contains unique features to allow for modeling the SHG response of nonlinear optical materials in the most general scenarios. We've made extensive efforts to design the GUI in a way to balance between the generality, efficiency, and user-friendliness.   

Key features of  **♯SHAARP**._ml_ include:  
- Flexibility of the sample structure 
	- Arbitrary number of layers 
	- Variable layer thickness 
- Flexibility in materials properties
	- Arbitrary crystallographic orientation 
	- General anisotropy of the linear and nonlinear dielectric susceptibilities 
		- with 32 point groups included 
		- with symmetry constraint applied automatically 
	- Supporting complex values of the coefficients for modeling absorbing materials  
- Flexibility in the wave setup   
	- Arbitrary incident angle, polarized state, wavelength of the incident wave
	- Choice of rotation/fixed schemes for polarizer/analyzer   
	- Built-in Fresnel coefficient and Maker fringes for parametric study   
	- Choice of assumptions made for SHG polarization 
		- With/Without consideration of the multiple reflection of fundamental waves 
		- Choice of contributions to the nonlinear polarization  
- User-friendliness 
	- Well-designed GUI 
	- Interactive 2D and 3D schematic illustration 
	- More than 10 case studies of common SHG materials included  
	- Allow user-defined new materials  
	- Copiable output plots and expressions 
	- Good efficiency 
		- Less than 1 min for single incident angle simulation 
		- Typically a few minutes for parametric studies such as Maker fringes/Fresnel coefficients 
- Programmable 
	- Modulized functions of the code 

In general, **♯SHAARP**._ml_ is designed to be useful for two types of studies:  
1. To simulate SHG responses of nonlinear optical materials/heterostructures 
2. To obtain analytical expressions of SHG responses and fit experimental measurements to determine the nonlinear optical properties of materials/heterostructures 

With given materials properties, **♯SHAARP**._ml_ allows for numerical simulation of SHG responses for arbitrary orientation of the crystal/sample, arbitrary optical polarization states of the incident wave, geometry considerations.

To obtain an analytical expression of the SHG response for a slab or multilayer consisting of nonlinear optical materials with unknown SHG coefficients and thickness. This expression can then be used to fit the SHG intensity measured from experiments,  from which one can extract structural information (e.g., thickness of the SHG active layer), determine the symmetry/polarity of the sample, and quantify the nonlinear optical susceptibilities (i.e., the SHG coefficients).

# Quickstart 
---
## Installation 

♯SHAARP._ml_ is written as a notebook using Wolfram Language and the access to _Mathematica®_ or *Wolfram Player* is required to run **♯SHAARP**._ml_ on PC/Mac. 

### Install _Mathematica®_ or *Wolfram Player* 
- To install Mathematica, please refer to the [Installing Mathematica](https://reference.wolfram.com/language/tutorial/InstallingMathematica.html)
- If you already have a Wolfram account, you can log in through the [portal](https://account.wolfram.com/login) and download the software.
- Wolfram player (to be test)
### Download the source code of **♯SHAARP**._ml_
- Download SHAARP.ml_V#.zip in the file list to start using ♯SHAARP.
	- The latest release (create link here)
- Unzip the file and you will obtain two notebooks: 
	- SHAARP.nb
	- setup.nb

## Run the GUI 
- Open SHAARP.nb and execute the initialization cell 
- run the GUI by executing run
- You will get the welcome page as: 


## Run the default case study 




## To learn more

Please refer to the documentation to learn more advanced topics and tips about **♯SHAARP**._ml_. 

---

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
1. R. Zu, B. Wang, J. He, J.-J. Wang, L. Weber, L.-Q. Chen, and V. Gopalan, SHAARP: An Open-Source Package for Analytical and Numerical Modeling of Optical Second Harmonic Generation in Anisotropic Crystals, (2023).
2. R. Zu, B. Wang, J. He, J.-J. Wang, L. Weber, L.-Q. Chen, and V. Gopalan, SHAARP: An Open-Source Package for Analytical and Numerical Modeling of Optical Second Harmonic Generation in Anisotropic Crystals, (2022).

## Acknowledgement
This development of the software was supported as part of the Computational Materials Sciences Program funded by the U.S. Department of Energy, Office of Science, Basic Energy Sciences, under Award No. DE-SC0020145.
