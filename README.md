# EEI6373 - Performance Modelling Mini Project

## Performance Modelling of a University Student Registration Queue Under Varying Arrival Rates

This is a mini project for **EEI6373 – Performance Modelling** at the Open University of Sri Lanka.

The project models a physical university student registration queue and evaluates its performance under different student arrival rates.

## System

The modeled system consists of:

- One registration officer
- One waiting queue
- First-Come, First-Served (FCFS) service discipline
- Students arriving for registration
- Registration service followed by departure from the system

The study focuses on the effect of increasing student arrival rates on the performance of the registration queue.

## Performance Objectives

The project focuses on the following performance objectives:

- Minimize student waiting time
- Maximize system throughput
- Identify performance bottlenecks
- Analyze queue length
- Evaluate registration officer utilization

## Workload Scenarios

Three workload scenarios are considered:

| Scenario | Arrival Rate |
|---|---:|
| Normal | 10 students/hour |
| High | 20 students/hour |
| Peak | 25 students/hour |

The average registration service time is approximately **4 minutes per student**.

## Dataset

A synthetic dataset is used because real operational data from the university registration office is not available for this study.

The dataset represents student arrivals and registration service times under the three workload scenarios.

## Simulation

The queue is modeled using a **discrete-event simulation** implemented in Python.

The simulation uses:

- Python
- NumPy for random data generation and simulation calculations
- pandas for data processing and result analysis
- Matplotlib for visualization

Each workload scenario is evaluated using **30 independent simulation replications**, with **100 students per replication**.

## Repository Structure

```text
EEI6373-PerformanceModelling-MiniProject/
│
├── analysis/
│   ├── EEI6373_Registration_Queue_Performance_Summary.csv
│   ├── EEI6373_Registration_Queue_Replication_Results.csv
│   └── registration_queue_simulation.ipynb
│
├── EEI6373_Registration_Queue_Synthetic_Dataset_Cleaned.csv
└── README.md
