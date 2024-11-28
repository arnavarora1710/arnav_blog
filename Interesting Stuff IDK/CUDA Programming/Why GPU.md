Better than CPU:
- Higher instruction throughput (how many instructions per cycle)
- More memory bandwidth (rate of i/o on data)

FPGAs etc. might be energy efficient but harder to program

- CPUs are designed to do ops sequentially and MAYBE do some of these ops in parallel
- GPUs are specialized to do 1000s of ops in parallel (sacrificing single-thread speed to get higher throughput)
	- More transistors devoted to processing than caching and optimizing control flow
	- Basically trying to brute force (amortizing) single-thread stuff to get better performance in parallel

Some things can obviously not be done in parallel : so we use a mix of sequential and parallel parts done with a mix of CPUs and GPUs.