# 470-gputsp
JMU CS470 Elective Project - TSP on GPUs

Use `update.sh` to pull repo + submodules after clone.

### Build Instructions
Most submodules have simple make files.

Concorde:
        
    ./configure --with-qsopt=$PWD/qsopt --enable-pthreads
    make 

to run

    ./TSP/concorde

### Submodules
* LOGO-solver: Main implementation analyzed - 2-opt local search, CPU and GPU
* acotsp: Ant Colony Optimization implementation - Implemented OpenMP parallel version
* concorde: Concorde Solver - branch and bound serial exact solver
* tsplib: problem sets

See READMEs for more information.

### Files
* `update.sh` - do the right pull for submodules
* `opt_tour.sh` - find the optimal tour for a problem set
* links - interesting reading material
* Traveling Salesman: Heuristic Scaling Analysis.pdf - final report

### Problem data
The tsplib submodule has TSPLIB formatted data sets.
Optimal solutions are also included there.
In any sub-folder the opt_tour.sh script can be run and passed a filename (without the .tsp) to return the optimal tour length from the solutions file.
