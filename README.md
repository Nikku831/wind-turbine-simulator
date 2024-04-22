# wind-turbine-simulator
This a simulink model for simulating a very basic wind turbine simulator based on the following mathematical formulae.

![image](https://github.com/Nikku831/wind-turbine-simulator/assets/132049110/6b5666d5-3772-4888-9717-232f5f4dc6a0)

### Power associated with wind turbine is given by the formula
P = ½ * C<sub>p</sub> (𝜆, β) * ρ * A * V<sub>w</sub><sup>3</sup>

where C<sub>p</sub> (𝜆, β) is Performance coefficient of wind turbine

𝜆 is optimal tip speed ratio 

β is blade pitch angle (degrees) 

ρ is air density (=1.225 kg/m3) 

A is the area swept by the blade (m2) 

V<sub>w</sub> is the wind speed 

### C<sub>p</sub> (𝜆, β) = C<sub>1</sub> * (C<sub>2</sub>/𝜆 - C<sub>3</sub> * β - C<sub>4</sub> * β<sup>2</sup> - C<sub>5</sub>) * e<sup>(-C<sub>6</sub>/𝜆<sub>i</sub>)</sup>

The values of C<sub>1</sub>, C<sub>2</sub>, C<sub>3</sub>, C<sub>4</sub>, C<sub>5</sub>, C<sub>6</sub>, β = 0.5, 116, 0.4, 0, 5, 21, 6 

𝜆<sub>i</sub> refers to intermittent tip speed ratio i.e. ratio between the tangential speed of the tip of a blade and the actual speed of the wind, V<sub>w</sub>. 

### 1/𝜆<sub>i</sub> = 1/(𝜆+0.08*β) - 0.035/(1+β<sup>3</sup>)

### 𝜆 = ω<sub>r</sub>*R/V<sub>w</sub>

ω<sub>r</sub> is represents rotational speed of shaft 

R is the radius of blade
# How to use
In order to give input, open the file in simulink and you can simply click the block and give repective inputs.

The outputs(power and torque) will be displayed in the end blocks.

Let me remind you again this simulator is very basic and simply simulates these mathematical equations.
