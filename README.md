Intelligent CPU Scheduler Simulator

Description:
The Intelligent CPU Scheduler Simulator is a tool designed to simulate various CPU scheduling algorithms.It provides real-time visualizations of scheduling processes, allowing users to input process details such as arrival time, burst time and priority. simulator generates Gantt charts and calculates key performance metrics like average waiting time and turnaround time

Features

*Support for multiple CPU scheduling algorithms:

*First Come First Serve (FCFS): 
  This is the simplest scheduling algorithm where processes are executed in the exact order they arrive. 
It works like a queue, where the first process to enter is the first one to get executed. 
However, if a long process arrives first, smaller ones must wait, leading to high waiting times. 
This can cause the convoy effect, where short processes suffer delays. 
While easy to implement, it is not always the most efficient method for optimizing CPU utilization.

*Shortest Job First (SJF): 
  This algorithm selects the process with the shortest burst time and executes it first. 
It reduces the overall waiting time and improves efficiency. However, SJF requires knowing the burst time in advance, which is not always possible. 
It has two variations: preemptive (where a shorter process can interrupt a longer one) and non-preemptive (where once a process starts, it completes before switching). 
The downside is that long processes may experience starvation if short jobs keep arriving.

*Round Robin (RR):
  Each process gets a fixed time slice (quantum) for execution before moving to the next process in a cyclic manner. 
This ensures fairness and prevents any single process from monopolizing the CPU. It is widely used in time-sharing systems. 
However, frequent context switching can add overhead, slowing down execution. If the quantum is too small, the CPU spends too much time switching tasks.
If it is too large, it starts resembling FCFS, losing its efficiency for quick response times.

*Priority Scheduling: 
  Each process is assigned a priority, and the CPU selects the process with the highest priority for execution. 
If two processes have the same priority, they follow FCFS order. 
This can be preemptive (where a higher-priority process interrupts a lower-priority one) or non-preemptive (where once a process starts, it runs until completion). 
A major drawback is starvation, where low-priority processes may never get executed. A solution is aging, which gradually increases the priority of waiting processes over time.

*Interactive user input for process details

*Real-time visualization of Gantt charts

*Performance metrics calculation

*User-friendly interface
