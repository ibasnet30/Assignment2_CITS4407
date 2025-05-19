# 📊 CITS4407 - Assignment 2: Board Games Dataset Analysis

## 🗂 Overview

This assignment consists of three Bash scripts written to process and analyze a dataset from BoardGameGeek. The dataset provides metadata about thousands of board games, including player counts, ratings, mechanics, and domains.

The tasks performed are:

1. **Data Quality Check** — Identify columns with missing values.
2. **Preprocessing** — Clean and transform the data for analysis.
3. **Analysis** — Extract insights and compute Pearson correlations.

---

## 📜 Scripts Summary

| Script Name   | Description |
|--------------|-------------|
| `empty_cells` | Counts empty fields in each column of a semicolon-separated file. |
| `preprocess`  | Cleans the dataset by: <br>• Converting `;` to tab<br>• Removing `\r` line endings<br>• Replacing commas in floats<br>• Removing non-ASCII chars<br>• Assigning new IDs for missing entries |
| `analysis`    | Answers the following questions:<br>1. What is the most popular mechanic?<br>2. What is the most common domain?<br>3. Correlation: Year Published vs Average Rating<br>4. Correlation: Complexity vs Average Rating |

---

## ▶️ How to Run the Scripts

Ensure you are inside the working directory with all scripts and input files.

```bash
./empty_cells bgg_dataset.txt ";"
./preprocess bgg_dataset.txt > clean.tsv
./analysis clean.tsv
