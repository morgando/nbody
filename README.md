# nbody


Program simulates the evolution of a galaxy using difference equations to estimate
the x, y, and z positions and x, y, and z velocities of stars. Refer to the document “N-Body v1“ on Athena
to see these equations along with their derivations. In order to see translations of the difference equations
along with how they are implemented within this program, see the comments for the findNextVelocity and findNextPosition
methods in the Nbody class. 

This file contains the following classes involved in the program in the same order they are listed:

(1) The RunSimulation class contains the main method of the program which creates an object
of type Nbody. The user may specify a file name, delta t value, and simulation duration
in this call to the constructor.

(2) The Nbody class contains the algorithm being used to run the simulation—check the comment for the Nbody constructor
to see a description of this algorithm.

(3) The Entity class represents the stars in the simulation. It contains methods that store, manipulate, and 
retrieve information about stars relevant to the simulation.

(4) The Vector class facilitates the storage and manipulation of three-dimensional position
and velocity data. The position and velocity instance variables of Entity objects are objects of type Vector.

In order to run a simulation, the user must provide information about stars within the simulation 
in a file. To see specifications about how the file must be structured, look at the precondition
in the constructor for the Nbody class.

Besides controlling the initial masses, positions, and velocities of stars in the simulation,
the user can customize the duration of the simulation and the length of time between subsequent
velocity/position estimations in the call to the Nbody constructor in the main method. 
Again, check the comment for the constructor of the Nbody class to see specifications about these parameters.

## @author Morgan Douglas
## @version 01/13/18

