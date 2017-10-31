# CQSim - A Trace-based Event-Driven Scheduling Simulator (version 2.0)
The version is a plug-in for plan-based scheduling using CQsim. The design uses simulated annealing (SA) for optimization. Given the current system state consisting of the start time, the expected runtime, and the resource usage for each running job, the plan-based scheduler generates an execution plan for the jobs in the waiting queue that assigns each waiting job a start time in order to minimize certain performance metric. Since the master branch CQsim is for queue-based scheduling, the waiting jobs are extracted from the job execution plan to the execution queue sorted by their planned start times, allowing the HPC system to start a job at the head of the executing queue upon its planned start time. The RS (random search) part is an alternative plan-based scheduling. The difference between RS and our plan-based scheduling is the "annealing" part. This version was originally developed by Xingwu Zheng at the Illinois Institute of Technology. Note: if you use the tool in your work, please cite the following paper: X. Zheng, Z. Zhou, X. Yang, Z. Lan, and J. Wang, "Exploring Plan-Based Scheduling for Large-Scale Computing Systems", Proc. of IEEE Cluster'16, 2016. 

