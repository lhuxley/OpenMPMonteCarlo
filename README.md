

## Monte Carlo Simulation of Throwing Darts at a Target

This program simulates the act of throwing darts at a target using Monte Carlo method. It generates a large number of random "dart throws" and calculates the number of darts that land inside each of the three holes in the target. The target is defined by the center coordinates and radius of three holes.

This program can be run with different settings to test the performance of the simulation. The number of trials in the simulation, the number of threads used in parallelization, and the ranges for the random numbers can be set as constants in the program.

## Compiling and Running

To compile the program, run the following command:

```
$ g++ -o prog dartboard_montecarlo.cpp -lm -fopenmp
```

The `-lm` flag links the `math` library and the `-fopenmp` flag links the OpenMP library.

To run the program with default settings, run the following command:

```
$ ./prog
```

To run the program with custom settings, you can set the constants in the program before compiling, or you can pass them as command line arguments:

```
$ ./programname numtrials numthreads
```

where `numtrials` is the number of trials in the Monte Carlo simulation and `numthreads` is the number of threads to use in parallelization.

## Output

The program outputs the number of darts that landed inside each of the three holes in the target, as well as the estimated area of each hole and the total execution time.

If the `CSV` flag is defined in the program, the program outputs a comma-separated value (CSV) file with the following columns:

- Number of trials
- Number of threads
- Execution time (seconds)
- Number of darts landed inside the first hole
- Number of darts landed inside the second hole
- Number of darts landed inside the third hole
- Estimated area of the first hole
- Estimated area of the second hole
- Estimated area of the third hole

## License

This program is released under the [MIT License](https://opensource.org/licenses/MIT).
