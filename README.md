# automaton-models
### Automaton Models of Discrete Event Systems - A Flexible Manufacturing System

This project was developed as a school project for the System Modelling and Analysis course. 

It consists on developing suitable automaton models using the DESUMA modelling package for a discrete event system.

### The System

The system consists of an input conveyor belt, two machines M1 and M2, and an assembly centre AC. Parts of a single type arrive one at a time on the conveyor belt, and are moved by a robot to a free machine for processing. Both machines have a capacity of one part, and perform the same operation, but processing times may vary. Once processed, parts from M1 or M2 are transferred to AC, where two parts are required to assemble the final product. The assembled product then leaves the system through an output conveyor belt. It is considered that there can be at most 3 parts being, or waiting to be, processed in the system at any given time.

### The Problem

Develop suitable automaton models for the input conveyor belt, machines M1 and M2, and the assembly centre AC, as well as two alternative models for the following routing policies:

* Arriving parts are placed in M1 if it is free. Otherwise, M2 is used as long as it is free.
* If both machines are free, parts are placed in the machine which became free first. Otherwise, they are placed in whichever machine is free, if there is such a machine.

Then, use those individual automata to build models for the whole system, for each different routing policy, and verify that the system is non-blocking.


### Problem Extension

Modify the automata for machines M1 and M2 to consider breakdown events, which may occur (only) when the machine is processing a part. Assume that a broken machine will appear to accept parts indefinitely, but without ever actually processing them.
