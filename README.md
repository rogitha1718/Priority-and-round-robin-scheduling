# EX NO 9 – Priority and Round Robin Scheduling

## Aim
To study the concepts of Priority and Round Robin scheduling.

## Domain / Use Case
Ambulance instrument monitoring system (GPS, HeartRate, Oxygen, ECG).

## Files
| File | Description |
|------|-------------|
| `ex9_partA_priority.c` | Part A – Priority scheduling |
| `ex9_partB_round_robin.c` | Part B – Round Robin scheduling (time quantum 2) |
| `ex9_partA_output.png`, `ex9_partB_output.png` | Program outputs |

## Part A – Priority Scheduling
Burst times 5, 3, 4, 6 and priorities 3, 1, 2, 1. The instruments are bubble-sorted by priority (smaller number = higher priority) and run in that order, printing start and finish times.

```bash
gcc ex9_partA_priority.c -o priority
./priority
```
![Priority output](ex9_partA_output.png)

## Part B – Round Robin Scheduling
Each instrument gets a time quantum of 2 units in circular order until its remaining time reaches 0.

```bash
gcc ex9_partB_round_robin.c -o rr
./rr
```
![Round Robin output](ex9_partB_output.png)

## Definitions
- **Priority Scheduling** – the CPU goes to the process with the highest priority (usually the smaller number).
- **Round Robin** – preemptive; each process gets a fixed time quantum and, if unfinished, goes to the back of the ready queue.

## Result
Implemented the concepts of Priority Scheduling and Round Robin Scheduling in C successfully.
