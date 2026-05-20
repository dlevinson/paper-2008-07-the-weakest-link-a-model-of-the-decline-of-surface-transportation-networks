This java-based program is developed based on Simulator Of Ultra-connected Network Degeneration (SOUND), which simulates
the growth of a transport network with more used links reinforced and less used ones depreciated.

A class named "TopologyIdentifier" is embedded in "NetworkDynamics.java" to identify the predefined connection
patterns of specified link types. Therefore, not all the files in the package are relevant to topology identification.
For more details, refer to Xie, Feng and David Levinson (2006) Measuring the Structure of Road Networks. Geographical Analysis (accepted)

The procedure to test "TopologyIdentifier" is the following:
1. Import the package into a java platform such as Eclipse.
2. Run the program as an applet. The main class is included in "Demo.java".
3. On the left-bottom corner of the applet, input the name of a test file and click "Load" to load the file.
The package includes four files for test, named "test-1","test-2","test-3","test-4", respectively.They are
actually the files that store the results of running SOUND experiments,which record the information of network topology,
speeds and volumes of each link at each round throughout the simulation of network growth.
4. After loading is completed, click ">" or "<" in the applete to examine the network structure at a specific
iteration. Step size can be chosen from a dropbox.
5. At the same time, the measures of connection patterns of arterial links (in yellow) every 5 iterations
have been printed out in the console window.

In the "TopologyIdentifier" class:
Output() method calculates the structual measures of network topologies for specified iterations;
identifySubgraph() identifies the unconnected pieces of arterials in a given network;
identifyCircuitBlocks() identifies the circuit blocks in the network;
identifyEnvelope() identifies the envelope of a given circuit block;
bridge() identifies bridge links;
articulation() identifies articulation points;
decompose() decompose a network into components by removing bridges and articulation points.

Refer to the notations in the codes for more details.