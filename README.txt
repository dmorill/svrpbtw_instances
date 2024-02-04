Folder Instances

It contains 4 instance folders: sets of 10, 15, 20, and 30 clients, respectively. Each instance has the following structure:

**The first line contains the total number of nodes including the depot.
**Starting from the second line, there are 7 columns containing the parameters of all nodes, starting with the depot data. Each column contains:
Column 1: X Coordinate (cm)
Column 2: Y Coordinate (cm)
Column 3: Demand (boxes)
Column 4: Service Time (min)
Column 5: Node Type (line 1 /back 0)
Column 6: Lower TW Limit (min)
Column 7: Upper TW Limit (min)

****In the case of the depot, the values will always be the same in all instances:
X Coordinate (cm): 0
Y Coordinate (cm): 0
Demand (boxes): 0
Service Time (min): 0
Node Type (line 1 /back 0): 0
Lower TW Limit (min): 0
Upper TW Limit (min): 1440 (indicating it is open all day)

**At the end of the parameters for all clients is the matrix of variations from one node to another. We set 5%, 15%, and 25%, where 5% means low variation in speed, 15% means medium variation, and 25% means high variation.

/////////////////////////////////////////////////////////////////////////

Folder Dats

It contains 4 folders: sets of 10, 15, 20, and 30 clients, respectively. Each folder contains the .dat files of deterministic instances, meaning instances that only have one scenario. The internal structure of each file is as follows:

param V1= number of clients;
param COST_cm=0.00451414 Cost per centimeter traveled (COP); (It is always the same value for all files)
param COST_min=2000 cost per minute traveled (COP); (It is always the same value for all files)
param K1= number of vehicles;
param M=9000000 (BIG M); (It is always the same value for all files)
param CV= 100000 vehicle utilization cost (COP); (It is always the same value for all files)
param U=2 vehicle capacity (boxes);
param Dem:= client demands (boxes)
;

param a:= lower TW limit (min)
;

param b:= upper TW limit (min)
;

param s: service time (min)
;

param D: distance matrix from one node to another (cm)
;

param t: travel time matrix from one node to another (min)


/////////////////////////////////////////////////////////////////////////

Escenarios Folder

It contains 4 folders: sets of 10, 15, 20, and 30 clients, respectively. Each folder contains the .dat files with the stochastic component, meaning they contain the generated scenarios. The internal structure of each file is as follows:

param N= number of scenarios;
param V1= number of clients;
param COST_cm=0.00451414 Cost per centimeter traveled (COP); (It is always the same value for all files)
param COST_min=2000 cost per minute traveled (COP); (It is always the same value for all files)
param K1= number of vehicles;
param FC=83333.3; //conversion factor that was not used but added to the files
param M=9000000 (BIG M); (It is always the same value for all files)
param CV= 100000 vehicle utilization cost (COP); (It is always the same value for all files)
param U=2 vehicle capacity (boxes);
param Dem:= client demands (boxes)
;

param a:= lower TW limit (min)
;

param b:= upper TW limit (min)
;

param s: service time (min)
;

param D: distance matrix from one node to another (cm)
;

param t: travel time matrix from one node to another (min)

param E:= matrix of times for each scenario
[,,1]:
