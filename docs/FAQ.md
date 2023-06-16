## initialization of ♯SHAARP._ml_ 
- Q: Why doesn't main panel show up?
- A: It usually takes 20 ~ 30s for the initialization depending on the configuration of hardware. 

## Warning message of ♯SHAARP._ml_ 
- Q: Why there are warning signs before progress bar?
- A: This is because the environment is not properly initialized. Go to <span style="background-color: #D3D3D3">Evaluation</span> → <span style="background-color: #D3D3D3">Evaluate Notebooke</span>. The warning sign should disappear.

## ♯SHAARP._ml_ gets stuck
- Q: Why does ♯SHAARP._ml_ get stuck in the calculation?
- A: This situation depends on the case you are working on. (1) Maker fringes and partial analytical expressions can be slow if the step size of Maker fringes is too fine (~0.02$^{\circ}$) or too many variables are involved. (2) If it is not the case in (1), it's recommended to close all the Mathematica notebook and reopen the ♯SHAARP._ml_.

## No variables in Partial Analytical Expressions
- Q: Why the generated expressions don't contain any variables? 
- A: This is because the variables have to be specified for certain layers. See [analytical thickness (h)](<input.md#Input panel##Functionality###Material thickness>) and [analytical SHG tensor (d)](<input.md#Input panel##Functionality###SHG tensor>).

## Output does not display properly in partial/full analytical expressions 
- Q: The output is cropped, and I can not see the full output
- A: This is because Mathematica will adjust the display of the output depending on the length of the expressions. Drag the small triangle button at the bottom right of the output page to adjust the view panel to see the full output.
>![BeforeDrag.png](img/BeforeDrag.png)
>The initial cropped display.


>![AfterDrag.png](img/AfterDrag.png)
>Display after adjusting the output size using the bottom right triangle 
## Initialization of SHAAP 
- Q: Cannot initialize `SHAARP_Init.nb` 
- A: Make sure the initialization notebook `SHAARP_Init.nb` is inside the same folder of `SHAARP_SI_Vxx.nb`. 
	- Otherwise, try to explicitly give the absolute path of `SHAARP_Init.nb`, just like 
