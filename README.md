## Description

The dataset contains 1050 problem instances for the multi-line permutation flow shop problem. The generation follows the method of Tallard (1993)[^fußnote] and generates random processing times in the interval [1,99]. To create the demand plan we draw randomly from a multinomial distribution with equal probability for each job type.

## Dataset structure

The PFSP dataset is structured in 15 folders. Each folder contains problem instances for a combination of line layout and processing time variation.

*Notation*: Tai_PFSP_**A**L_**B**
**A**: Number of Lines (1-3)
**B**: Number of processing time variation (1-5)

Each folder contains 70 problem instances. A problem file is a combination of one problem characteristic (number of jobs, machines and stations) and a demand plan variation. The processing times are fixed for one problem characteristic. 

*Notation*: t**CD**\_**E**\_**F**\_**G**\_**H**.mix
**C**: Number of Lines (1-3)
**D**: Number of problem characteristic (1-7)
**E**: Number of jobs (20,100,500)
**F**: Number of machines (5,10,20)
**G**: Number of sorts (5,10,20)
**H**: Number of demand plan variation (1-10)

Each file represents a different problem file in text format.

*Line Notation*:
L1: Demand plan 
L2: Layout Type
L3: Number of machines
L4: Number of machines per line
L5: Number of total machines with synchronization machine
L6: Number of sorts
L7-end: Processing times matrix for the combination of machine (row) and job type (column)

[^fußnote]: Taillard, E. (1993). Benchmarks for basic scheduling problems. European Journal of Operational Research, 64 (2), 278{285.