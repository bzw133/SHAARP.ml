![GitHub release version](https://img.shields.io/github/v/release/bzw133/SHAARP.ml?color=%2350C878&include_prereleases)
![License](https://img.shields.io/github/license/Rui-Zu/SHAARP)
![GitHub Size](https://img.shields.io/github/repo-size/bzw133/SHAARP.ml)
[![HitCount](https://hits.dwyl.com/bzw133/shaarpml.svg?style=flat-square)](http://hits.dwyl.com/bzw133/shaarpml)
[![HitCount](https://hits.dwyl.com/bzw133/shaarpml.svg?style=flat-square&show=unique)](http://hits.dwyl.com/bzw133/shaarpml)
# Welcome to ♯SHAARP._ml_ 

**♯SHAARP**._ml_ is an open-source package for modeling reflected and transmitted optical second harmonic generation (SHG) of a single-layer slab and multi-layer heterostructure of nonlinear optical materials. 

This package builds in the most general approach to both analytically and numerically solving the SHG response of various materials systems. The package is designed to handle **arbitrary number of layers, number of SHG active mediums, crystal symmetry, arbitrary orientation, complex refractive indices, and arbitrary polarization state of light** (e.g., linearly, circularly, elliptically polarized). The two most common SHG characterization approaches, Maker fringes and polarimetry, are integrated into the package. 

**♯SHAARP**._ml_ is also a successor of the **♯SHAARP**._si_, which was designed for modeling the reflected SHG responses for an single interface.  

!!! note
		The single interface package (**♯SHAARP**._si_) can be accessed using links: [GitHub](https://github.com/Rui-Zu/SHAARP), [Manual](https://shaarp.readthedocs.io/en/latest/) and [Tutorial Videos](https://www.youtube.com/watch?v=fr0RirVHXVc)


# A primer of the theoretical background  

As a very brief primer, Optical SHG describes the process where two photons of frequency $\omega$ interact with a nonlinear medium to create a photon at 2$\omega$, so called the SHG process. 

The SHG is induced by a quadratic dielectric response, given by $P_i^{2\omega} = d_{ijk}E_j^{\omega}E_k^{\omega}$, where $E$ is the fundamental electrical field of the fundamental wave at $\omega$ frequency, $P^{2\omega}$ is the nonlinear polarization at $2\omega$ frequency created inside the crystal, and $d_{ijk}$ is a third rank polar tensor describing the nonlinear optical property of the crystal. The subscripts _i, j, k_ are dummy subscripts running from 1 to 3. The SHG tensor, $d_{ijk}$, has 3x6=18 independent non-zero components in general considering the interchangeable indices of the electric field term $E_j^{\omega}$ and $E_k^{\omega}$ . The crystal symmetry can further reduce the number.

There are four sets of coordinate systems used in **♯SHAARP**._ml_. Namely, the crystallographic, the crystal physics, the principal, and the lab coordinate systems. The crystallographic coordinate refers to the the crystallographic axes $(a,b,c)$ for a unit cell which does not necessarily to be orthogonal to each other depending on the crystal system. The crystal physics coordinate system is orthogonal with three axes denoted as $(Z_1,Z_2,Z_3)$ in **♯SHAARP**._ml_. The principal coordinate system contain three axes $(Z_1^{principal},Z_2^{principal},Z_3^{principal})$ and is extensively used to describe the optical properties of crystals such as optical axis and refractive indices. They are similar but not identical to the crystal physics coordinate system. The lab coordinate system with the axes $(L_1,L_2,L_3)$ determine the set up the model. We adopt the convention that the plane of incidence coincides with the $L_1-L_2$ plane, and the incident light is propagating toward the positive direction of $L_3$.  

Beside the three 3D coordinate systems, another 2D coordinate system is useful to describe the polarization state of a wave, namely, the polarizer/analyzer coordinate system (?). The two axes (_s_, _p_) are orthogonal, with s axis is perpendicular to the plane of incidence and p axis is within the plane of incidence. The plane expanded by *s* and *p* axes is perpendicular to the wavevector of the wave entering the polarizer/analyzer.  

A clear understanding of the relationships between these concepts is highly recommended to successfully employ **♯SHAARP**._ml_ to obtain reasonable results and draw reliable comparison with experiments. We have tried to make it clear for new users by incorporating several interactive 2D and 3D illustrations in the GUI. 


# Project outline

### [Install](install.md)
### [Getting Started with ♯SHAARP._ml_](getstarted.md)
### [Methods](methods.md)
### [Inputs](input.md)
### [Outputs](output.md)
### [Examples](examples.md)
### [Frequently Asked Questions](FAQ.md)
