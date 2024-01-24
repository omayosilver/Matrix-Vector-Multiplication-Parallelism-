# Matrix-Vector-Multiplication-Parallelism-
This is a course test for parallel programming by Dr Yulan Jan 2024

This repository contains the parallel Open MPI and OpenMP implementation of Matrix-Vector Multiplication using the Row-wise striped method. 

To run, please do the following:

Please set the following ENV variables on the terminal where you will be running the script. If you're using bash shell:

export rows=<number of matrix rows>
export cols=<number of matrix cols>
export proc=<number of processes>
export FUNCTIONAL_MODE=<As Below>
FUNCTIONAL_MODE

0 => Output the graphs for a different number of processes (which can be added in `scripts/report.sh` file)

1 => Use the Row-wise method to calculate matrix-vector Multiplication

sh make.sh

This will first make all the files present in the src/
The results would be either in graphs or a report according to the FUNCTIONAL_MODE selected.
Each code also contains a validation step where the output of both parallel and serial implementation of MVM are compared. An error is reported if the results don't match.
