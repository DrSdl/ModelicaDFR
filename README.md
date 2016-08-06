# ModelicaDFR
A package for Modelica simulating Molten Salt Reactors

The package contains a "SingleFluidMoltenSaltReactor" and a "DualFluidMoltenSaltReactor" model. Both models make use of a "PointKineticMoltenSaltReactor" class. 

Modelica has not been used a lot in the nuclear industry so far - which is a pity in my opinion. Computer codes like TRACE, ATHLET or RELAP are much more widely used and are very specialized for light water reactor applications. But their software architecture is outdated from a 21st century point of view. Modelica uses an object oriented approach for system modeling and it is easy to swap one fluid property for another one like molten salts. It is also easy to extend the fluid properties and connectors to new classes being able to track the movement of neutron precursor atoms in the primary circuit. 

And when it comes to simulate for example the behavior of reprocessing units attached to a molten salt reactor Modelica offers all the framework which is necessary to do so. No upside without downside: since Modelica does not a priori know which kind of system you are going to simulate the numerical solver cannot be as specialized as in the case of TRACE or RELAP. This may result in longer integration times or in much difficulty finding suitable initial guesses.

The other big advantage of Modelica is that it is an open standard and that there are open source solvers like JModelica or OpenModelica available to immediately jump into simulations. Of course, when you do these simulations every day in and out you would want to have a professional and robust solver like Dymola.

For the details of the models please have a look at the comment block at the start of each model in this package. I have done here a quick approach in order to make a proof-of-principle demonstration that Modelica can be used for the system simulation of molten salt reactors. My hope is that students in the future will develop a much more sophisticated package.

Two video tutorials have been produced which can be accessed by the following links and which help you to start building on the Nuclear.mo models:

Tutorial 01: Very Basic Introduction
https://s3-eu-west-1.amazonaws.com/ms-01-s3bucket/DFR_tutorial_part01.html

Tutorial 02: Simulate with JModelica
https://s3-eu-west-1.amazonaws.com/ms-01-s3bucket/DFR_tutorial_part02.html

Some useful links:

Modelica Standard: https://www.modelica.org/

Modelica by Example: http://book.xogeny.com/

JModelica: http://www.jmodelica.org/

OpenModelica: https://www.openmodelica.org/

Dymola: http://www.3ds.com/products-services/catia/products/dymola







