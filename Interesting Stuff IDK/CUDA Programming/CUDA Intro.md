"A General-Purpose Parallel Computing Platform and Programming Model"

Allows usage of C++ for programming

[[List of Main Abstractions in CUDA|3 key abstractions]]:
1. thread groups
2. shared memories
3. barrier synchronization

Partition the problem into sub-problems that can be solved independently in parallel by blocks of threads, and each sub-problem into finer pieces that can be solved cooperatively in parallel by all threads within the block

So, this kinda means that you are allocating independent jobs to blocks but maybe-not independent jobs to threads within blocks

Can be scaled horizontally easily (just increase blocks)