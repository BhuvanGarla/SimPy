# SimPy
Simulating a container terminal

# Container Terminal Simulation

This project uses common Python modules along with SimPy to simulate operations at a container terminal.

## Task Overview

The intention is to imitate ships pulling into the container terminal. With an average of five hours, the intervals between vessel arrivals follow an exponential distribution. There are 150 containers on each vessel that need to be emptied. Berthing, using quay cranes for unloading, and using terminal trucks to move containers to yard blocks are all part of terminal operations.

## Simulation Details

1. **Vessel Arrivals**:
    - Vessels arrive at the terminal following an exponential distribution with an average interval of 5 hours.
    - Each vessel carries 150 containers.

2. **Berths**:
    - The terminal has 2 berths. If both are occupied, arriving vessels must wait.

3. **Quay Cranes**:
    - There are 2 quay cranes available.
    - Each crane can move a container in 3 minutes.
    - A crane must wait for an available truck to transport the container.

4. **Terminal Trucks**:
    - There are 3 trucks available for transporting containers from the quay cranes to the yard blocks.
    - Each truck takes 6 minutes to drop off a container and return.

5. **Logging**:
    - Events such as vessel arrival, berthing, crane operations, and truck operations are logged with timestamps.

## Requirements

- Python 3.x
- SimPy

## Installation

To install SimPy, run the following command:

```bash
pip install simpy

