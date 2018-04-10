# EE564 Project-2

## Motor Winding Design & Analysis

## Deadline 23/04 23:59

## Grading and Procedure

See the [Evaluation](./evaluation.md) sheet for details.

### Lamination Selection

In the project folder you'll find the several induction motor laminations from [Kienle Spiess](http://www.kienle-spiess.de/induction-machines.html). Please select a lamination. Although, students are allowed to work on same laminations, I don't want close friends to work on the same lamination. I expect you to work independently, and there is no difference of difficulty between laminations. 

You can find the definitions of the parameters in the legend file. You can also get registered in [Kienle Spiess](http://www.kienle-spiess.de/induction-machines.html) to get extra information. Throughout the assignment, please ignore small features of the drawings (i.e. drill holes, shaft opening etc).

You can use any material for your laminations, but please refer to the data-sheet of the laminations you choose.


## Q1) Winding Design

For the lamination you had chosen, depending on the number of stator slots and rotor slots, design a winding diagram including but not limited to:

- Number of poles
- Type of winding (integral, fractional, single layer, double layer etc.)
- Winding diagram
- Winding factors (including first few harmonics)
- Number of turns, and wire size
- Fill factor
- Winding connection (delta-wye)
- Rated phase current

For the winding you selected please plot the MMF waveform for two different instants for a balanced three-phase current (i.e. Ia=1 A, Ib=-0.5 A, Ic=-0.5A)

## Q2) Motor Parameter Estimation





In this assignment you are required to design and analyze an inductor wrapped around a toroidal core. You are free to choose any type of material, but at least find a decent [manufacturer](https://www.mag-inc.com/Products/Ferrite-Cores/Ferrite-Toroids), so you have a detailed data-sheet of the toroid core.

Choose a number of turns, and current so that the core operates in the linear region, but just close to saturation with DC excitation. Again you are free to choose any combinations, but choose reasonable values. Do NOT copy from each other.

### Part A - Analytical Calculations

1- Calculate the inductance of the coil assuming the flux is homogeneously distributed, and there is no leakage flux, and the core is linear (i.e. constant permeability).

2- Calculate the inductance when the flux is NOT homogeneously distributed, and there is no leakage flux, and the core is linear.(Hint: You can divide the core in discretized cylindrical sections)

3- Repeat parts 1 and 2 by assuming the core is non-linear and the DC current is increased by 50%.

Now assume you opened a 2mm air-gap in the toroid as shown below:

![](https://img1.exportersindia.com/product_images/bc-full/dir_117/3493672/gapped-toroidal-core-2002349.jpeg)

4- Repeat part 1 by assuming there is NO fringing flux.

5- Repeat part 1, but this time propose a method to estimate the effect of the fringing flux and calculate the inductance.

### Part B - Finite Element Analysis

In this part you will repeat the calculations you did in part A using a FEA software.

Here are a few suggestions:

- You can use any software you want, please have a look at the [course page](http://keysan.me/ee564)

- If you haven't used any FEA software before, I advise you to start with FEMM, which is free and a simple program. If you are planning to use FEA simulations in your professional life, then it makes sense to learn a more capable program (e.g.  Maxwell)

- 2D simulations will be enough for assignments in this course, but if you feel comfortable you can proceed with 3D simulations (but you have been warned).

- You can approximate the coils by solid copper regions (i.e. you don't have to model each number of turns),  but if you want you can model each coil as a bonus.

- There are a few expert users in the class, if you feel stuck, please ask for help. The solution is usually very simple.

1- Analyze to core in magneto-static (DC current, steady-state) using linear magnetic magnetic properties (i.e constant permeability). Show the flux density distribution in the core. Don't forget to include air-region around the core.

2- Calculate total inductance, and leakage inductance (you can use the magnetic energy stored in the core and in the air region to estimate these values).

3- Repeat parts 1 and 2 with non-linear material properties.

4- Now, with non-linear material properties, include the airgap and show the effect of the fringing flux, and also calculate the inductance for this geometry. 

### Part C- Discussion

In this part, compare all the analytical and FEA inductance calculations in a table and discuss the differences.

Also discuss the differences between 2D and 3D FEA simulations (you don't have to make 3D simulations, just discuss which effects are ignored in 2D simulations).


## Q2) Transformer Design

In this question you are going to repeat the analytical transformer design you did in the class. The specs are:

- 500 kVA, Single Phase
- 34.5kV/25 kV
- 50 Hz
- Ambient Temp: -30C-50C

However this time, you are required to do a more detailed analysis regarding the material, core geometry, number of turns, equivalent circuit parameters etc.

I want you to come with an optimum design, but also discuss the effect of a few design parameters (i.e. different lamination types, varying number of turns etc.)

Please present all relevant parameters of your design, values of the equivalent circuit parameters, cost, efficiency etc.






