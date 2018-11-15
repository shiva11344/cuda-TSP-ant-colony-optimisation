
# Travel Salesman Problem using Ant Colony Optimization
### shiva swaroop. v
### sree charan. M


## Instructions for TSP using ACO ==> Ant Colony Optimization.

* For ACO , since it's a much smaller and simpler code , I just used 1 file each for parallel and CUDA version. I'm using an    open source map_generator (coded in ruby), that takes the number of cities as a parameter and builds a map.txt that contains a random city map with said N cities. 
Command to run the map generator : ruby map_generator.rb Num_of_cities
* I have compiled and saved 3 different variants of maps for the ease of the grader to check my code. map25.txt , map50.txt , and map100.txt contains maps with 25,50,100 cities respectively.

* To run the sequential and parallel version of the code. 
 ### Just do a 'make'
  and to run the sequential version using 
 ### for example to run for 25 cities -> ./tsp-ant-cpu < map100.txt
  and to run the parallel version using
 ### for example 25 cities -> ./tsp-ant-gpu < map100.txt
  This ensures that the input data for parallel and sequential version is same

### NOTE: Just like GA, even in this, to play around with a number of cities, just open ants.c - line 7 & parallel_ants.cu - line 8and change the #define cities 25 , to whatever value you want ,25,50 or 100 and do a 'make' to compile the code. Since all the memory allocation and some other global variables depend on the 'CITIES' variable, I didn't take it as a parameter and instead defined it as a #define.


* Happy Testing :) 
