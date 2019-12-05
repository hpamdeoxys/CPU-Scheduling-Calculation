# CPU Scheduling Calculation
Simulate FCFS, SJF, SRTF, and Round Robin Scheduling Algorithms.
Compute Waiting Time and Turnaround Time of Every Job and Average Waiting Time and Turnaround Time.
Show Ghant Chart

## Summary
Project was created as part of Operating System class final project. Data Structures used are Dictionaries and List; Which are built-in Python. Choice of Python language was simple due to math computation and ease use of mutable objects.

## Output
```OUTPUT
FIRST COME FIRST SERVE
| KEY | ARRIVAL | BURST | WAIT | TURNAROUND |
  P1       0       10       0        10
  P2       1        2       9        11
  P3       4        4       8        12
  P4       5        1      11        12
  P5      10        3       7        10
  P6      21       12       0        12
Average Wait Time = 5.833333333333333    Average Turnaround Time = 11.166666666666666

0 -> P1 -> 10 -> P2 -> 12 -> P3 -> 16 -> P4 -> 17 -> P5 -> 20 -> P6 -> 33 

SHORTEST JOB FIRST
| KEY | ARRIVAL | BURST | WAIT | TURNAROUND |
  P1       0       10       0        10
  P2       1        2      10        12
  P3       4        4      12        16
  P4       5        1       5         6
  P5      10        3       3         6
  P6      21       12       0        12
Average Wait Time = 5.0    Average Turnaround Time = 10.333333333333334

0 -> P1 -> 10 -> P4 -> 11 -> P2 -> 13 -> P5 -> 16 -> P3 -> 20 -> P6 -> 33 

SHORTEST REMANING TIME FIRST
| KEY | ARRIVAL | BURST | WAIT | TURNAROUND |
  P1       0       10       1        11
  P2       1        2      10        12
  P3       4        4      12        16
  P4       5        1       4         5
  P5      10        3       3         6
  P6      21       12       0        12
Average Wait Time = 5.0    Average Turnaround Time = 10.333333333333334

0 -> P1 -> 9 -> P4 -> 10 -> P1 -> 11 -> P2 -> 13 -> P5 -> 16 -> P3 -> 20 -> P6 -> 33 

ROUND ROBIN QT=4
| KEY | ARRIVAL | BURST | WAIT | TURNAROUND |
  P1       0       10       7        17
  P2       1        2       3         5
  P3       4        4       2         6
  P4       5        1       9        10
  P5      10        3       7        10
  P6      21       12       0        12
Average Wait Time = 4.666666666666667    Average Turnaround Time = 10.0

0 -> P1 -> 4 -> P2 -> 6 -> P3 -> 10 -> P1 -> 14 -> P4 -> 15 -> P1 -> 17 -> P5 -> 20 -> P6 -> 25 -> P6 -> 29 -> P6 -> 33 
```

## Goal
* Add Context Switching
* Random Number of Process and Values (Given Constraint)
* Choice of Display
