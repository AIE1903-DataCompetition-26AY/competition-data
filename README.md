# Wireless Network Traffic Forecasting Competition

## Overview

This competition focuses on **wireless network traffic forecasting** using uplink traffic time series sampled at **5-minute intervals**.

To accommodate students with different levels of experience, the competition provides **three difficulty levels**. Students may choose the dataset that best matches their interests and modeling ability.

## Difficulty Levels

| Level | Dataset | Description |
|---|---|---|
| **Beginner** | **30 Selected Cells** | A subset of 30 cells with relatively clear and stable traffic patterns. Recommended as the starting point for students who are new to time-series forecasting. |
| **Intermediate** | **217 Full Cells** | The complete set of 217 cells. Some cells have more irregular or less favorable temporal characteristics, making the task more challenging and requiring greater model robustness. |
| **Advanced** | **273 Grids** | The 30 selected cells are further divided into 273 spatial grids. This setting provides finer-grained traffic series and is the most challenging level. |

The three levels are related as follows:

```text
217 Full Cells
   └── 30 Selected Cells
          └── 273 Grids
```

## Dataset Files

Each difficulty level is provided in a separate folder. Each folder contains:

- a **training set**;
- an **empty test set** containing the timestamps and required prediction columns;
- a **baseline / sample submission file**;
- a **PDF data description** containing detailed information about the dataset, task, evaluation metrics, and submission requirements.

The **273-grid dataset** additionally contains:

```text
grid_cell_membership.csv
```

which records the correspondence between each grid and its parent cell.

## Getting Started

Choose one of the three difficulty levels, read the corresponding **PDF data description**, and use the provided training and test files to build your forecasting model.

For detailed dataset statistics, field definitions, train/test splits, evaluation metrics, and submission rules, please refer to the PDF included in each dataset folder.
