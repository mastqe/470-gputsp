# 470-gputsp
JMU CS470 Elective Project - TSP on GPUs

Clone using `git clone --recursive` to get all submodules.

If not cloned recursively use 

    git submodule init
    git submodule update

To pull updated submodules

    git pull --recurse-submodules

### Build Instructions
Most submodules have simple make files.

Concorde:
        
    ./configure --with-qsopt=$PWD/qsopt --enable-pthreads
    make 

to run

    ./TSP/concorde

### Problem data
The tsplib submodule has TSPLIB formatted data sets.
Optimal solutions are also included there.
In any sub-folder the opt_tour.sh script can be run and passed a filename (without the .tsp) to return the optimal tour length from the solutions file.
