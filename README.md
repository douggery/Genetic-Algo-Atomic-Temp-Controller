# Gentic-Algo-Atomic-Temp-Controller
Control systems course project using genetic algorithms to optimize a temperature controller for atomic clocks


The attached pdf used matlab to simulate the step response of a digital control system 
to control the temperature of a small vapor cell used in chip-scale atomic clocks. 

Lumped-element modeling was applied to estimate the transfer function and using 
standard/textbook stability criteria, the initial parameters are set.

Using a genetic algorithm for simplicity, the control parameters were modified
and the fitness tested which penalized overshoots and rise times. 

Genetic algos are pretty dumb but in this case they were sufficient to implement
a solution that didn't care that the underlying system was intrinsically nonlinear
(due to actuator saturation). 

The python pycontrol module can implement these functions for linear systems and
a finite time response can be implemented to simulate nonlinear systems

If done again, I would at least modify the genetic algo to become evolutionary
by decreasing the mutation rate over time. 
