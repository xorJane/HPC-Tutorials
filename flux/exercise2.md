---
layout: default
title: "Exercise 2"
release_number:
author: Ryan Day, Lawrence Livermore National Laboratory
---

## Exercise 2: Launching and tracking job steps
1. Ensure that you have a flux instance running in an allocation and determine the number of cores available to you in that allocation.
2. Download the attached `mpi_hellosleep.c` file and build the application with `mpicc -o mpi_hellosleep mpi_hellosleep.c`.
3. Run `mpi_hellosleep` as a blocking job step with enough mpi tasks to fill all of the cores available in your flux instance.
4. Submit two non-blocking job steps that will run `mpi_hellosleep` with enough mpi tasks to fill all of the cores available in your flux instance. Verify that only one of the job steps is running.
5. Cancel the running job step. Confirm that the other job step is running and attach to it to monitor its progress.

### Notes / Solutions
1. See [Exercise 1](exercise1).
2. On LC systems, mpicc should be in your default path. If it is not, you can run `module load intel` and `module load mvapich2` to get the default mpicc on most LC systems.
3. See 'Submit blocking job steps' in [Section2](section2).
4. See 'Submit non-blocking job steps' in [Section2](section2).
5. See 'Managing job steps' in [Section2](section2).