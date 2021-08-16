# CPI-Stack-Estimation-

In this exercise we are required to obtain the CPI (Cycles Per Instruction) stack for programs using hardware performance monitoring counters.
CPI stack divides the total CPI of an application into components that reflect the time spent in various events, such L1-I Cache misses, L1-D cache misses, L2/L3 Cache misses, I-TLB and DTLB misses, branch misprediction, etc. (See [1] for details regarding CPI Stack).		
The counts of various miss events occuring during program execution can be obtained using hardware Performane Monitoring Counters (PMC) on modern architectures.		
(See [2] for details regarding PMCs available on Intel Skylake Processor).		
Performance counter values for running application can be obtained using performance monitoring tools such as PAPI [3] or perf [4].


We are required to run a set of programs on your laptop/desktop and collect performance counter values for various events. You are required to develop a simple linear regression model (using simple linear terms) for CPI for each application. 

References:
[1]		A	Top-Down	Approach	to	Architecting	CPI	Component	Performance	Counters Article		in		IEEE	Micro	·	February	2007
[2]	 Intel®	 64	 and	 IA-32	 Architectures	 Software	 Developer’s	 Manual - Volume 3B: System	Programming	Guide, Part 2
[3]PAPI	User’s	Guide. Available	at:	
http://icl.cs.utk.edu/projects/papi/files/documentation/PAPI_USER_GUIDE_23.htm
[4]	Linux	Kernel	Profiling	with	perf. Available	at:
https://perf.wiki.kernel.org/index.php/Tutorial
