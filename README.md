## Description

Two datasets are provided. The main dataset (folder data) contains 1050 problem instances for the multi-line permutation flow shop problem. The generation follows the method of Tallard (1993) and generates random processing times in the interval [1,99]. To create the demand plan we draw randomly from a multinomial distribution with equal probability for each job type. 

The additional dataset (folder data_disturbed) contains 150 problem instances for the multi-line permutation flow shop problem with short term-disturbances.

## Dataset structure

Each PFSP dataset is structured in 15 subfolders. Each folder contains problem instances for a combination of line layout and processing time variation.

*Notation*: Tai_PFSP_**A**L_**B** / Tai_D_PFSP_**A**L_**B** <br/>
**A**: Number of Lines (1-3) <br/>
**B**: Number of processing time variation (1-5) <br/>

Each folder contains 70 problem instances. A problem file is a combination of one problem characteristic (number of jobs, machines and stations) and a demand plan variation. The processing times are fixed for one problem characteristic. 

*Notation*: t**CD**\_**E**\_**F**\_**G**\_**H**.mix <br/>
**C**: Number of Lines (1-3) <br/>
**D**: Number of problem characteristic (1-7) <br/>
**E**: Number of jobs (20,100,500) <br/>
**F**: Number of machines (5,10,20) <br/>
**G**: Number of sorts (5,10,20) <br/>
**H**: Number of demand plan variation (1-10) <br/>

Each file represents a different problem in text format.

*Line Notation*: <br/>
L1: Demand plan <br/>
L2: Layout Type <br/>
L3: Number of machines <br/>
L4: Number of machines per line <br/>
L5: Number of total machines with synchronization machine <br/>
L6: Number of sorts <br/>
L7-end: Processing times matrix for the combination of machine (row) and job type (column) <br/>

1. Taillard, E. (1993). Benchmarks for basic scheduling problems. European Journal of Operational Research, 64 (2), 278-285.