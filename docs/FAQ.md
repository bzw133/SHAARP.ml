## Good practice when using ♯SHAARP._ml_
- It is recommended one should **NOT** save the SHAARP._ml_.nb.
- All postprocess should be performed in a separate notebook. 
- If for any reason you would like to save SHAARP._ml_.nb, always "Delete All Output" (from the drop-down menu `Cell` of Mathematica) before saving. Otherwise, there will issues with the preexisting "ghost" GUI when re-opening the same notebook next time.

## Initialization of ♯SHAARP._ml_ 
- Q: Why doesn't main panel show up?
- A: It usually takes up to 20 ~ 30s for the initialization depending on the configuration of hardware.
- Q: Cannot initialize `SHAARP_Init.nb` 
- A: Make sure the initialization notebook `setup.nb` is inside the same folder of `SHAARP.ml.nb`. 

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

- Note 1: If the expression is too large to show, ♯SHAARP._ml_ will automatically hide it. The user can Export it into a ".mx" file and save to local by click the "Export" button. Then the "*.mx" file can be import in a separate notebook even after closing the ♯SHAARP._ml_ notebooks. 
- Note 2: If the expression is too large to show, "Copy" is not recommended because it may cause crush of Mathematica. Please use "Export" instead and then Simplify it. 

## Mathematica crushes when executing ♯SHAARP._ml_ (Error messages keep printing out and never cease even click Abort) 
- When this happens, you will have to either kill the process of Mathematica software or the Wolfram Kernel in the Task Manager. In either case, you will lose the unsaved status of the notebook.    
