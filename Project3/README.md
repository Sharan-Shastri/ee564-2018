# EE564 Project-3

## Motor Design Project

## Deadline 04/06 23:59

## Grading and Procedure

See the [Evaluation](./evaluation.md) sheet for details.

## Projects

In this project#3, you'll have three options to select from:

## A-Traction Motor Design

The motor you need to design is a traction asynchronous squirrel cage induction motor (with copper rotor-bars) with the following specifications:

- Rated Power Output: 1280 kW
- Line-to-line voltage: 1350 V
- Number of poles: 6
- Rated Speed: 1520 rpm (72 km/h) (driven with 78 Hz inverter)
- Rated Motor Torque:   7843 Nm
- Cooling: Forced Air Cooling
- Insulating Class: 200C
- Train Wheel Diameter: 1210 mm
- Maximum Speed: 140 km/h
- Gear Ratio: 4.82

You can find some reference analytical designs from the [Github repo](https://github.com/odtu/ee564/tree/master/TRAIN). Although you are free to use this as a reference, do not copy anything. Reports and source code will be checked by Turnitin

## B- Wind Turbine Generator Design

You are required to design a squirrel cage induction generator for the Northel Energy's VIRA-250 wind turbine. The specifications of the wind turbine are as follows:

- Rated Power: 250 kW
- Rated Wind Speed:  14 m/s 
- Rated Turbine Speed: 24.3 rpm
- Gear Ratio: 31.2
- Number of Poles: 8
- Line to line voltage: 400 V
- Frequency: 50 Hz
- Rated Speed: 758 rpm
- Gearbox: (Coupled from wind turbine blade)
- Insulation Class: F

You can find some reference analytical designs from the [Github repo](https://github.com/odtu/ee564/tree/master/WIND). Although you are free to use this as a reference, do not copy anything. Reports and source code will be checked by Turnitin


## C-Alternate Design for your 2nd Project

You are required to re-analyze the motors you used for your 2nd project, but you are required to complete a more detailed analysis (details given below), and I would lke you to evaluate the effect of one parameter you choose such as:

- What happens if you use a different rotor/stator slot configuration
- What happens if you increase/decrease the airgap length
- What happens if you choose a different winding design.
- What happens if you design a different rotor/stator slot shape

### Design Scope

The outputs of the projects are as follows:

Analytical Section:

(Note if you have already calculated these in your project#2, you can refer to that project):

- Design your motor anayltically, and determine the main dimensions. Put your calculations in your design report. Please include some basic drawings.
- Decide on the material properties, mechanical frame size etc.
- Calculate the magnetic circuit parameters (flux density calculations at various points: air-gap, teeth, back-core etc, magnetic loading)
- Electric Circuit (Winding selection, electric loading, fill factor, phase resistance, winding factors (for fundamentalsn and for harmonics)).
- Rough thermal calculations (cooling method, operating temperature, ways to improve cooling)
- Efficiency, current, torque characteristics
- Mass Calculations (structural mass, copper mass, steel mass etc)

Compulational Section:

You are supposed to model the induction machines you designed analytically and in FEA. You are free to use any FEA software, but I advise you to use Maxwell.

- Model your design to RMxprt.
- In the RMxprt get the performance metrics such as: (torque vs. speed, flux in the airgap, cogging torque etc).
- Export your design into Maxwell 2D (don't bother with 3D simulations)
- In 2D FEA show the flux density distribution, flux vectors. Calculate the flux densities in the critical parts (tooth, back core etc)
- Compare the FEA results with your analytical calculations
- Also I expect you to comment on general design considerations that you learnt throughout the course.

## Useful Software

Apart from the analytical calculations you are required to use software tools to verify your calculations.

- [ANSYS Maxwell](https://www.ansys.com/products/electronics/ansys-maxwell): Especially the RmXprt toolbox of Maxwell will the most useful option. You can also use Maxwell 2D simulations for flux density calculations.
- [MotorAnalysis](http://motoranalysis.com/): A free MATLAB GUI for induction motor design. Although it may be slow for some cases, it is easy to use and simple tool.
- [Dolomites](https://sourceforge.net/projects/dolomites/): It has a few useful design snippets that you can refer.

There are also other software you can use in the course web page.
