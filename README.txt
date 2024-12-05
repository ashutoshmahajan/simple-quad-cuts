This file describes the data collected from the computational experiments described in Section 6.1, Section 6.2 of the manuscript titled "Cutting planes from the simplex tableau for quadratically constrained problems" by Mustafa Vora and Ashutosh Mahajan.

This supplementary material consists of two files, DatasetT1.csv and DatasetT2.csv in the comma separated values (csv) format. These can be read using a text editor or a spreadsheet-based software. Below are the details of each file.

1. DatasetT1.csv
This file contains results of all experiments on the instances in set T1 described in the manuscript. It has 165 rows, including one header row and one row for each instance, and the following 27 columns.
- Instance: Name of the instance.
- (MCS) Time in cutting: Total time (in seconds) taken in cut generation and solving the subsequent LP in Minimum Coefficient Sum (MCS) variant.
- (MCS) Cuts added: Number of cuts added in MCS.
- (MCS) Gap closed: Percent gap closed in MCS, computed using Equation (9) in the manuscript.
- (EW) Time in cutting: Total time (in seconds) taken in cut generation and solving the subsequent LP in Equal Weight (EW) variant.
- (EW) Cuts added: Number of cuts added in EW.
- (EW) Gap closed: Percent gap closed in EW, computed using Equation (9) in the manuscript.
- (RCW) Time in cutting: Total time (in seconds) taken in cut generation and solving the subsequent LP in Reduced Cost Weight (RCW) variant.
- (RCW) Cuts added: Number of cuts added in RCW.
- (RCW) Gap closed: Percent gap closed in RCW, computed using Equation (9) in the manuscript.
- (LI) Time in cutting: Total time (in seconds) taken in cut generation and solving the subsequent LP in Least Infeasible (LI) variant.
- (LI) Cuts added: Number of cuts added in LI.
- (LI) Gap closed: Percent gap closed in LI, computed using Equation (9) in the manuscript.
- (MS) Time in cutting: Total time (in seconds) taken in cut generation and solving the subsequent LP in Most Sparse (MS) variant.
- (MS) Cuts added: Number of cuts added in MS.
- (MS) Gap closed: Percent gap closed in MS, computed using Equation (9) in the manuscript.
- (ObO) Time in cutting: Total time (in seconds) taken in cut generation and solving the subsequent LP in One-by-One (ObO) variant.
- (ObO) Cuts added: Number of cuts added in ObO.
- (ObO) Gap closed: Percent gap closed in ObO, computed using Equation (9) in the manuscript.
- (S2V) Time in cutting: Total time (in seconds) taken in cut generation and solving the subsequent LP after variable addition when both variables are substituted (S2V).
- (S2V) Relative size: The relative size of the new relaxation in S2V.
- (S2V) Gap closed: Percent gap closed in S2V, computed using Equation (9) in the manuscript.
- (S1V) Time in cutting: Total time (in seconds) taken in cut generation and solving the subsequent LP after variable addition when one variable is substituted at a time (S1V).
- (S1V) Relative size: The relative size of the new relaxation in S1V.
- (S1V) Gap closed: Percent gap closed in S2V, computed using Equation (9) in the manuscript.
- SCIP Default: The percent change for default SCIP, computed using Equation (10) in the manuscript.
- SCIP No heuristics: The percent change for SCIP with no heuristics, computed using Equation (10) in the manuscript.

2. DatasetT2.csv
This file contains results of all experiments on the instances in set T2. It has 77 rows, including one header row and one row for each instance, and the following 5 columns.
- Instance: Name of the instance.
- (ObO) Time in cutting: Total time taken in cut generation and solving the subsequent LP in One-by-one (ObO) variant.
- (ObO) Cuts added: Number of cuts added in ObO.
- SCIP Default: The percent change for default SCIP, computed using Equation (10) in the manuscript.
- SCIP No heuristics: The percent change for SCIP with no heuristics, computed using Equation (10) in the manuscript.

In both the files:
- A (*) in the 'Gap closed' column means the solver faced numerical issues for that variant.
- A (TL) in the 'Time in cutting' column means the solver was terminated on taking more than 9600s for that variant.
- A (#) in the SCIP Default or SCIP No heuristics column denotes that SCIP was terminated on taking more than 9600s while processing the root node. The bounds reported at the time of termination are included.
