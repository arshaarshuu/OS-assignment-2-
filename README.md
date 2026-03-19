
Description: Non-Preemptive Priority CPU Scheduling
This program implements the non-preemptive priority CPU scheduling algorithm in C. In this scheduling method, each process is assigned a priority value, and the CPU is allocated to the process with the highest priority (i.e., larger priority number indicates higher priority).

Working Principle:
Each process has:

Process ID (PID)

Arrival Time (AT)

Burst Time (BT)

Priority (PR)

At any given time, among all the processes that have arrived and are not yet completed, the process with the highest priority is selected for execution.

Since the algorithm is non-preemptive, once a process starts executing, it runs until completion without interruption.

If no process is available at the current time, the CPU remains idle until the next process arrives.

Calculations:
Completion Time (CT) = Time at which a process finishes execution

Turnaround Time (TAT) = CT − AT

Waiting Time (WT) = TAT − BT

Output:
Waiting time for each process

Turnaround time for each process

Average waiting time

Average turnaround time

Special Notes:
In case of a tie in priority, the process with the earlier arrival time is selected.

The program dynamically updates time and tracks completed processes to ensure correct scheduling.
