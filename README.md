# wind-turbine-simulator
A very basic wind turbine simulator
This a simulink model for simulating a very basic wind turbine simulator. The simulator is based on the formula.

Power associated with wind turbine is given by the formula
P= ½ * Cp (𝜆, β) * ρ * A * Vw^3
where Cp (𝜆, β) is Performance coefficient of wind turbine   
𝜆 is optimal tip speed ratio 
β is blade pitch angle (degrees) 
ρ is air density (=1.225 kg/m3) 
A is the area swept by the blade (m2) 
Vw is the wind speed 

Cp (𝜆, β) = C1 * (C2/𝜆 - C3 * β - C4 * β^2 - C5) * e^(-C6/𝜆i)
The values of C1, C2, C3, C4, C5, C6, β = 0.5, 116, 0.4, 0, 5, 21, 6 
𝜆i refers to intermittent tip speed ratio i.e. ratio between the tangential speed of the tip of a blade and the actual speed of the wind, Vw. 

1/𝜆i = 1/(𝜆+0.08*β) - 0.035/(1+β^3)

𝜆 = ωr*R/Vw
ωr is represents rotational speed of shaft 
R is the radius of blade

Let me remind you again this simulator is very basic and simply simulates these mathematical equations.
