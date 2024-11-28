# 2D Closed Trajectories Dataset

This repository contains multiple closed, non-intersecting 2D trajectories. Each trajectory's points are stored in a separate file and are ordered chronologically.

## Data Format

Each trajectory file is located in the `data` folder and follows the format:

- **File Format**: Plain text (`.txt`)
- **Data Shape**: `(N, 2)`
  - `N`: Number of points in the trajectory
  - Each row represents a 2D point: `[x, y]`

## How to Use

You can load the trajectory data in Python using the following code:

```python
import numpy as np

# Replace `data_name` with the name of the trajectory file (without the extension)
traj_data = np.loadtxt("./data/{}.txt".format(data_name))
