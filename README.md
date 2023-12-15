# Repeating Mathematical modelling and simulation of the thermo-catalytic decomposition of methane for economically improved hydrogen production:
## Background and Paper Reference: 
Brock Lumbers a, David W. Agar b, Joachim Gebel a, Frank Platte; Mathematical modelling and simulation of the thermo-catalytic decomposition of methane for economically improved hydrogen production. International Journal of Hydrogen Energy (Mathematical modelling and simulation of the thermo-catalytic decomposition of methane for economically improved hydrogen production - ScienceDirect).

The objective of this project is to repeat and enhance the model developed in the above paper. Hydrogen is a clean and sustainable energy carrier, and green hydrogen production methods are critical for reducing greenhouse gas emissions. The thermo-catalytic methane decomposition (TCMD) process is a promising intermediate solution that generates no direct carbon dioxide emissions and can bridge the transition to green hydrogen whilst utilizing existing gas infrastructure.  
The motivation for choosing this subject is directly related to the huge ongoing effort in industry to produce green hydrogen and minimize greenhouse gas emission to achieve the world climate goals. This paper presents a study of hydrogen production utilizing the thermo-catalytic methane decomposition (TCMD) process:
Below list of ODEs that I will utilize from the paper to perform my analysis: 

![image](https://github.com/AhmedJabbari/ChE2410-Project-2/assets/148829971/0ec9a78c-f60e-4a99-8225-6a943e74794d)


The values of the parameters that I will analysis from the paper are kT=-0.05 (1/s), v= 1 (m^3/s), x=0.78, W=100 (kg) and Q=50 (J/s). In this analysis I will only concentrate on hydrogen production despite the fact that the paper presented several results and models for several components. The model and experimental data that were found in the paper can be seen below: 

![image](https://github.com/AhmedJabbari/ChE2410-Project-2/assets/148829971/695fccfc-0a80-481a-929c-470937a29164)

## Optimizing Parameters and Model Fitting

Firstly, I plotted the experimental data and the model fit to evaluate if they are directly fitting or not. As shown in the below figure the experimental data and the model data fit are not fitting together.  

![image](https://github.com/AhmedJabbari/ChE2410-Project-2/assets/148829971/0f6c4496-ba95-45cb-9b2a-ea6d76481361)

 
Then, I utilized curve fit function from Python to fit the model. As shown in the below figure there is an improvement in fitting the experimental data and the model but it is still there is a difference between experimental data and the model after fitting. 

![image](https://github.com/AhmedJabbari/ChE2410-Project-2/assets/148829971/2e093f25-7156-4fdf-89de-96c003e0c912)

 
The parameters after fitting and optimization are kT=-0.011 (1/s), v= 0.65 (m^3/s), x=0.01, W=98.9 (kg) and Q=2.03e+07 (J/s). After comparing the optimized parameters after fitting with parameters from paper we can clearly see that there is minor to moderate discrepancies for kT, v, x and W parameters and there is huge discrepancy for Q parameter. These minor to moderate discrepancies may be due to the fact the experiment was conducted on Packed Bed Reactor while the model in the paper was developed on CSTR reactor. As for the Q parameter it could be a typing mistake. Therefore, there is an area for improvement to narrow down to more accurate values.
