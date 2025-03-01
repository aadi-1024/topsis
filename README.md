# TOPSIS Score Calculation

This project calculates the Technique for Order of Preference by Similarity to Ideal Solution (TOPSIS) score for a given dataset. TOPSIS is a multi-criteria decision-making method.

## Requirements

- Python 3.x
- pandas
- numpy

Install the required packages using pip:

```bash
pip install pandas numpy
```

## Usage

To run the script, use the following command:

```bash
python3 main.py <input> <weights> <impacts> <output>
```

### Parameters

- `input`: Input CSV file containing the dataset.
- `weights`: String of weights for each criterion, separated by commas.
- `impacts`: String of impacts for each criterion (`+` for beneficial, `-` for non-beneficial), separated by commas.
- `output`: Output CSV file for saving the results.

## Example

```bash
python3 main.py data.csv '2,1,1,1,1' '+,-,+,+,+' out.csv
```

## Input Data Format

The input CSV file should have the following format:

| Identifier | Criteria1 | Criteria2 | Criteria3 | Criteria4 | Criteria5 |
|--|-----------|-----------|-----------|-----------|-----------|
| Id1 | Value1    | Value2    | Value3    | Value4    | Value5    |
| ... | ...       | ...       | ...       | ...       | ...       |

## Output

The output CSV file will contain the original data along with the calculated TOPSIS scores and rankings.