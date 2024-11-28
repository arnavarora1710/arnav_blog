- Defined by \_\_global\_\_  declaration specifier
- Also needs the number of CUDA threads that execute this specific kernel for a given kernel call
	- Defined by <<<...>>>

Each thread being used in the kernel is given a unique ID (accessible using built-in variables)
