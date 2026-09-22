# Scheduling Optimization – Genetic Algorithm

A Python-based scheduling optimization project developed as part of my Industrial Engineering and Management studies.

The project solves a single-machine scheduling problem with the objective of minimizing total earliness and tardiness penalties.

Two solution approaches are implemented:
- Mathematical optimization using PuLP
- Genetic Algorithm (GA)

## Project Overview

Each job is defined by:
- Processing time
- Due date
- Earliness penalty
- Tardiness penalty

The objective is to determine an efficient job schedule that minimizes the total penalty associated with completing jobs before or after their due dates.

## Genetic Algorithm

The Genetic Algorithm searches for improved job sequences using:

- Population generation
- Fitness evaluation
- Rank-based selection
- Crossover
- Mutation
- Survivor selection
- Iterative improvement under a configurable time limit

Each chromosome represents a possible ordering of the jobs. The algorithm evaluates different schedules and retains the best solution found during the optimization process.

## Mathematical Optimization

PuLP is used to formulate and solve the scheduling model.

The model includes:
- Job start and completion times
- Earliness and tardiness variables
- Non-overlapping job constraints
- Weighted earliness and tardiness penalties
- Penalty minimization objective

## Input & Output

The program reads scheduling data and Genetic Algorithm parameters from Excel files.

The generated Excel output includes:
- Job sequence
- Start and completion times
- Earliness and tardiness
- Penalty per job
- Total penalty
- Number of GA generations
- Runtime
- Gantt-style schedule visualization

## User Interface

A Tkinter-based GUI allows the user to:
- Choose between the Genetic Algorithm and mathematical solver
- Specify input and output files
- Run the optimization process

## Technologies

- Python
- Pandas
- PuLP
- OpenPyXL
- Tkinter
- Genetic Algorithms
- Mathematical Optimization

## Repository Structure

```text
Scheduling-Optimization-Genetic-Algorithm/
├── app.py
├── genetic_algorithm.py
├── optimization_solver.py
├── requirements.txt
├── .gitignore
└── README.md
```

## How to Run

Install the required packages:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python app.py
```

## Skills Demonstrated

- Python programming
- Optimization modeling
- Genetic Algorithms
- Operations Research
- Data processing with Pandas
- Excel automation
- Algorithm design
- GUI development
