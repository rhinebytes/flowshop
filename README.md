Flow shop
=========
Flow shop scheduling problems, are a class of scheduling problems with a work shop or group shop in which the flow control shall enable an appropriate sequencing for each job and for processing on a set of machines or with other resources 1,2,...,m in compliance with given processing orders. Especially the maintaining of a continuous flow of processing tasks is desired with a minimum of idle time and a minimum of waiting time. Flow shop scheduling is a special case of job shop scheduling where there is strict order of all operations to be performed on all jobs. Flow shop scheduling may apply as well to production facilities as to computing designs. A special type of flow shop scheduling problem is the permutation flow shop scheduling problem in which the processing order of the jobs on the resources is the same for each subsequent step of processing.
# Glossary
    * Makespan: Time between start and finish of a sequence of jobs
    * LB: Makespan best solution Lower Bound
    * UB: Makespan best solution Upper Bound
    * NEH: Algorithm by Nawaz, Enscore, Ham
    * IG: Iterated Greedy algorithm
    * ALT: Alternative algorithm
    * RPD: Relative Percentage Deviation
# Hints
    * Existing Taillard instances are ta001, ta002, ta003, ta004, ta005, ta006 etc.
    * Existing alias names for multiple Taillard instances are 20x5, 20x10, 20x20 etc.
    * Run alternative algorithm by implementing run method as described in file nop
    * Common values for parameter T of IG algorithm are 0.0, 0.1, 0.2, 0.3, 0.4 and 0.5
    * Common values for parameter d of IG algorithm are 2, 3, 4, 5, 6, 7 and 8
    * Common values for parameter ms of IG algorithm are 20 and 60
    * Set array of 10-digit numbers to overwrite initial seeds
# Examples
    flowshop 20x5 20x10 alt=./src/nop.js repeat=2 seed=auto
    flowshop ta001 ta002 ta003 seed=[1111111111,9999999999]
    flowshop 50x5 ta005 ta020 T=0.4 d=4 ms=20
    
    Usage: flowshop <INSTANCES SEPARATED BY SPACES> [alt=path/file]
    [T=N.N] [d=N] [ms=NNNN] [repeat=NN] [seed=[S1,S2,...,Sn]|auto|default]
