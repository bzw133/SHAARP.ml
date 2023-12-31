## Maker fringes

The following tutorial demonstrates the calculation of Maker fringes for a multilayer composed of Z-cut quartz with a gold layer deposited at the back of the slab. This example has been presented in the manuscript and highlights the importance of multiple reflections. 

We start by discussing the experimental details before proceeding to simulate the Maker fringes pattern. The multilayer comprises of a 121.2 $\mu$m thick Z-cut quartz with a 13.9 nm gold coating at the back. The fundamental wave is p-polarized and it's wavelength is set to 800 nm in air and the p-polarized SHG intensities are measured. Now, we discuss the simulation part below.

- Open `SHAARP.ml_Vx.xx.nb` in _Mathematica®_. Evaluate the notebook by clicking `Evaluation > Evaluate Notebook`. Ensure that Dynamic Evaluation is enabled in _Mathematica®_. If everything goes right, the user guide should be visible in the notebook as shown below.

   ![good](./img/good.png)
   In case the above is not seen, please re-evaluate the notebook or restart _Mathematica®_ and try again.

-  In the functionality sub-panel of the input panel on the left, click `Set Material Properties` to define the multilayer.

- Set the wavelength to 0.8 $\mu$m (800 nm) from the wavelength setting sub-panel.

- In the `Material Selection` sub-panel, type 2 for the number of layers. 

- Click on `1` to edit the first layer of the multilayer. Give it a suitable name, say "Z-cut quartz". The crystal and optical properties of quartz are already pre-defined and saved as an example. To apply these properties, click on `Quartz (001)` from the case study sub-panel.

- From the `Material thickness` sub-panel, enter 121.2 ($\mu$m) to set the thickness of the quartz slab. Since the crystal and optical properties of quartz are already defined, nothing needs to be changed in the crystal structure, crystal orientation, dielectric tensors and SHG tensor sub-panels.
!!! note
	   In general, the user would need to manually enter the crystal and optical properties of the layer. See the Input Panel section of the manual for more details and instructions.

- Having defined the properties for quartz, now click `2` in the material selection sub-panel to set the properties of the gold layer. Give it a suitable name, say "gold" and click `Au coating` from the case study sub-panel. Now set the thickness to 0.0139 (13.9 nm). The other properties for the gold layer have already been provided. In general, the user would need to enter the values corresponding to the crystal and optical properties.

- Now click on `Update` to visualize the multilayer that has been defined. It should look like the figure below. 

   ![qAu](./img/qAu.png)

   The figure below the multilayer shows the relative orientation of the $Z_1 Z_2 Z_3$ axes of the selected layer with respect to the lab coordinate system $L_1 L_2 L_3$. From the functionality sub-panel, click on `3D Schematics` to see this as an interactive 3D figure.

- Now click on `SHG Simulation` in the functionality sub-panel to define the experimental setup. Check  `Generate Maker Fringes Plot` to calculate the Maker Fringes pattern.

- The full multiple reflection considering backward propagating waves along with standing waves is used for the simulation.

- In the Maker fringes collection settings, enter the incident angle range for the Maker fringes simulation. We shall simulate the pattern for incident angles between 0$^{\circ}$ and 45$^{\circ}$. To do this, set the minimum incident angle to 0 and maximum incident angle to 45. This can be done by either dragging the sliders, clicking on the angle button or manually entering the angle.

- Set the scan step size to 0.1$^{\circ}$ to see the intensity oscillations clearly. 

- As already described in the experimental setup above, the incident fundamental light is p-polarized and the p-polarized SHG intensity is to be recorded. Hence, set the polarizer angle $\varphi$ as well as the analyzer angle $\psi$ to 0. The incident ellipticity is 0 since the light is linearly polarized.

- Now click on `Update` to start the simulation. This shall take a few minutes due to the small step size. The simulated Maker fringes pattern should look as shown below.

	![makerpattern](./img/makerpattern.png)

-  Click `Copy` to copy the underlying list to the clipboard. In a *Mathematica®* notebook, paste this and give this a name. This list can now be plotted using `ListPlot[]`.

    !!! note
    	It is recommended to allow #SHAARP.ml finish running before running any other _Mathematica®_ notebook. 

-  One can also try changing the thickness of the slab by $\pm$1 $\mu$m to see the effect of the slab thickness on the Maker fringes pattern. To do this, go back to the `Set Material Properties` and click on `1` to modify the quartz layer. Change the thickness and click `Update`. Now click on `SHG Polarimetry` and click `Update` again to run the Maker fringes simulation for the new thickness.

## SHG Polarimetry

In this section, we show how two SHG active layers can be used to determine the spontaneous polarization by SHG interference contrast. The experimental setup consists of a 50 $\mu$m layer of LiNbO<sub>3</sub> ($2 \bar{1} \bar{1} 0$) crystal on 35 $\mu$m (001) quartz. The fundamental light has a wavelength of 1550 nm and is incident on the multilayer normally. The polarization of the fundamental light is varied and the p-polarized SHG intensity is recorded. To set the direction of the spontaneous polarizations (along c axis), it is easier to specify the orientation using the crystal physics coordinate system $Z_1 Z_2 Z_3$. 

![pols](./img/pols.png)

- Open `SHAARP.ml_Vx.xx.nb` in _Mathematica®_. Evaluate the notebook by clicking `Evaluation > Evaluate Notebook`. Ensure that Dynamic Evaluation is enabled in _Mathematica®_. If everything goes right, the user guide should be visible in the notebook. In case the user guide is not seen, please re-evaluate the notebook or restart _Mathematica®_ and try again.

- In the functionality sub-panel of the input panel on the left, click `Set Material Properties` to define the multilayer.

- Set the wavelength to 1.55 $\mu$m (1550 nm) from the wavelength setting sub-panel.

- In the material selection sub-panel, type 2 for the number of layers.  

- Click on `1` to edit the first layer of the multilayer. Give it a suitable name, say "LNO". The crystal structure and optical properties of LiNbO<sub>3</sub> are already pre-defined and saved as an example. To apply these properties, click on LiNbO<sub>3</sub> (0001) from the `Case Study` sub-panel.

- From the `Material thickness` sub-panel, enter 50 ($\mu$m) to set the thickness of the LiNbO<sub>3</sub> slab. Since the crystal structure and optical properties of LiNbO<sub>3</sub> are already defined, nothing needs to be changed in the crystal structure, dielectric tensors and SHG tensor sub-panels. 

!!! note
	In general, the user would need to manually enter the crystal and optical properties of the layer. See the Input Panel section of the manual for more details and instructions.

- To define the orientation of the LiNbO<sub>3</sub> crystal, click on `Use Crystal Physics Direction` in the crystal orientation sub-panel. For the spontaneous polarization of LiNbO<sub>3</sub> to be oriented along the polarization vector for quartz, the crystal physics vectors in the lab coordinate system take the following values: $Z_1 = (0,0,1)$, $Z_2=(0,-1,0)$ and $Z_3=(1,0,0)$. 

- Having defined the properties for LiNbO<sub>3</sub>, now click `2` in the material selection sub-panel to set the properties of the quartz layer. Give it a suitable name, say "quartz" and click `Quartz (001)` from the case study sub-panel. Now set the thickness to 35 ($\mu$m). The other properties for the quartz layer have already been provided. In general, the user would need to enter the values corresponding to the crystal and optical properties.

- Now click on `Update` to visualize the multilayer that has been defined. It should look like the figure below. 

	![LNOq](./img/LNOq.png)
The figure below the multilayer shows the relative orientation of the $Z_1 Z_2 Z_3$ axes of the selected layer with respect to the lab coordinate system $L_1 L_2 L_3$. From the functionality sub-panel, click on `3D Schematics` to see this as an interactive 3D figure.

- Click on `SHG Polarimetry` in the functionality sub-panel to generate the polar plots. If required, check `Generate Fresnel Coefficients Plot` and/or `Generate Maker Fringes Plot` to calculate the Fresnel coefficients and/or Maker fringes pattern.

- The full multiple reflection considering backward propagating waves along with standing waves is used for the simulation.

- From the polarimetry settings sub-panel, set the incident angle to 0 (normal incidence). Since the incident light is linearly polarized, the ellipticity is 0.

- The experiment describes a rotating polarizer, fixed analyzer geometry. Hence, click on `Rotate Polarizer` and `Fix Analyzer` in the polarimetry sub-panel. Since only the p-polarized SHG intensity is required, set the analyzer angle $\psi$ to 0.

- Click `Update` to run the SHG simulation and generate the polar plots. The resultant plots should look as shown.

	![polarplots](./img/polarplots.png)

- Now, to generate the polar plots for the case where LiNbO<sub>3</sub> polarization is opposite to that of quartz, go back to `Set Material Properties` and select the LiNbO<sub>3</sub> layer by clicking `1` in the materials selection sub-panel. 

- In the crystal orientation sub-panel, click `Use Crystal Physics Direction` and enter the following: $Z_1 = (0,0,1)$, $Z_2=(0,1,0)$ and $Z_3=(-1,0,0)$. 

- Now click `Update` and go to `SHG Polarimetry` and click `Update` again to generate the polar plots under the same polarimetry settings. One observes that the SHG plots have changed.

- To compare the intensities of both the configurations in the same plot, click `Partial Analytical Expression` and enter the same polarimetry settings used for SHG simulation. Click `Update` to obtain the expressions of the SHG intensities. For intensities polarized along $L_1$, copy $I^{T, 2 \omega}(\varphi, \psi)$ by clicking `Copy` next to it and assign it to a _Mathematica®_ function. Repeat the same for the other orientation and assign it to another _Mathematica®_ function. 

    !!! note
    	The expressions provided by clicking `Copy` below the SHG polar plots return normalized expressions, and is thus not suitable for intensity comparisons; hence we use the expressions provided by `Partial Analytical Expression` tab.

    !!! note
    	It is recommended to allow #SHAARP.ml finish running before running any other _Mathematica®_ notebook. 

- Now use `PolarPlot[]` to plot both of these on the same plot: 

    ![compp](./img/compp.png)

- Similarly, to compare the intensities of SHG polarized along $L_2$, copy  $I^{T, 2 \omega}(\varphi, \psi + \pi/2)$ and follow the same instructions outlined above. The plot would look like the one shown below (note the scaling factor):

    ![comps](./img/comps.png)

- One can also verify that the absence of the quartz layer results in the same SHG intensities for both the polarizations. To do this, go back to `Set Materials Properties` and remove the second layer and copy the expressions for the transmitted SHG intensities. Repeat the same for the other direction of polarization (by changing the crystal physics coordinates) and save these as *Mathematica*® functions and use `PolarPlot[]` to plot them.

## Partial Analytical Expressions

This section explains how to obtain the reflected and transmitted SHG intensities analytically so that comparisions to experiments can be made to either determine the point group or unknown SHG coefficients by fitting. For this tutorial, we choose a material "similar" to quartz whose thickness is unknown. This material differs from quartz only with respect to it's SHG tensor elements, with $d_{11}=0.3$ and unknown $d_{14}$. Fundamental light of 800 nm is assumed to be incident at 45$^{\circ}$ on this material. The experimental setting is a rotating polarizer and fixed analyzer.

- Open `SHAARP.ml_Vx.xx.nb` in _Mathematica®_. Evaluate the notebook by clicking `Evaluation > Evaluate Notebook`. Ensure that Dynamic Evaluation is enabled in _Mathematica®_. If everything goes right, the user guide should be visible in the notebook. In case the user guide is not seen, please re-evaluate the notebook or restart _Mathematica®_ and try again.
- In the functionality sub-panel of the input panel on the left, click `Set Material Properties` to define the material.
- Set the wavelength to 0.8 $\mu$m (800 nm) from the wavelength setting sub-panel.
- In the material selection sub-panel, type 1 for the number of layers.  
- Click on `1` to edit the first layer of the multilayer. Give it a suitable name, say "quartz". The crystal structure and optical properties of quartz are already pre-defined and saved as an example. To apply these properties, click on quartz (001) from the `Case Study` sub-panel.
- In the thickness sub-panel, click `analytical h` to provide a variable thickness to the slab. The box should show `h1`.
- In the SHG tensor sub-panel, click `analytical dij`. This will replace all the text boxes with unknown coefficients `d11m1` and `d14m1`. For the point group 32, there are only two independent SHG coefficients $d_{11}$ and $d_{14}$. Since it's given that $d_{11}=0.3$, manually enter this value in place of `d11m1`. This effectively leaves only one undetermined SHG coefficient $d_{14}$. One may also leave all the SHG coefficients as symbolic variables and finally substitute them with the numerical values. However, due to more unknowns in this case, it takes a longer time to calculate the analytical expressions.
- Click `Update` to visualize this quartz slab.
- In `Partial Analytical Expressions`, enter the assumption to use. In this case, full multiple reflections with backward waves and standing waves will be considered. 
- Set the incident angle to $45^{\circ}$ and set the polarimetry configuration to rotate polarizer and fix analyzer. 
- Click `Update` to generate the SHG intensities as a function of unknowns `h1` and `d14m1`.
- Click `Copy` to copy any of the expressions and assign it to a function with variables $\varphi$, `h1` and `d14m1`. Use `Simplify[]` to simplify the expression if required. The final statement will look like `funcName[\[CurlyPhi]_, h1_, d14m1_] := Simplify[ *paste here* ]`. This function can be used as a regular *Mathematica®* function.

!!! note
	$\varphi$ (`\[CurlyPhi]`) can be quickly entered in *Mathematica®* using the alias `Esc-j-Esc`.

!!! note
	In some cases, the derived expressions are too long to be displayed. In this case, the output panel displays "Too long to show". However, the user can still click `Copy` (`Export`)  to copy (export) the full expression.

!!! note
	It is recommended to allow #SHAARP.ml finish running before running any other _Mathematica®_ notebook.   

-  Click `Export` to save the expression in a `.mx` file. Give it a suitable name while saving. 

-  To load the expression, use `Import[]`. Use the following code if the `.mx` file is saved in the same directory as that of the notebook:
![import](./img/import.png)
  
   If the `.mx` file is saved in a different directory from the one where the current notebook is being executed, enter the path of the saved file in the `Import[]` function.
  
   

