# Assignment 2 - CITS4407

Scripts:

- `empty_cells`: Counts empty cells in a semicolon-separated file
- `preprocess`: Cleans the dataset into tab-separated format and fixes decimals, encoding, IDs
- `analysis`: Performs data analysis including:
  - Most popular mechanics
  - Most common domain
  - Correlation between year & rating
  - Correlation between complexity & rating

## How to run

```bash
./empty_cells bgg_dataset.txt ";"
./preprocess bgg_dataset.txt > clean.tsv
./analysis clean.tsv
