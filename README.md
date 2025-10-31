# Power BI F1 Dashboard

This Power BI Dashboard provides an interactive view of Formula 1 World Championship data (1950–2020) using a dataset from Kaggle.

It enables detailed exploration of races, drivers, constructors, and circuits across seven decades of Formula 1 history.

![Circuits & Races](img\Circuits&Races.png)

![Constructor Insights](img\ConstructorInsights.png)

![Driver Performance](img\DriverPerformance.png)

## Dashboard Highlights

- Season Overview: Interactive breakdown of races, wins, and points per season.
- Driver Analysis: Career stats, podium finishes, nationality, and performance trends.
- Constructor Insights: Team dominance and evolution across decades.
- Circuit Map: Visual distribution of circuits worldwide.
- Historical Comparison: Explore year-by-year performance and championship results.

## Dataset

```python
# Install dependencies as needed:
# pip install kagglehub[pandas-datasets]
import kagglehub
from kagglehub import KaggleDatasetAdapter

# Set the path to the file you'd like to load
file_path = ""

# Load the latest version
df = kagglehub.load_dataset(
  KaggleDatasetAdapter.PANDAS,
  "rohanrao/formula-1-world-championship-1950-2020",
  file_path,
  # Provide any additional arguments like 
  # sql_query or pandas_kwargs. See the 
  # documenation for more information:
  # https://github.com/Kaggle/kagglehub/blob/main/README.md#kaggledatasetadapterpandas
)

print("First 5 records:", df.head())
```

## Dependencies

| Software          | Dependency Type   |
| ----------------- | ----------------- |
| Power BI Desktop  | Template (.pbit)  |
| Power BI Desktop  | Theme (.json)     |
| Kaggle            | Dataset Source    |
| Python (optional) | kagglehub, pandas |

## Setup Instructions

1. Download or clone this repository.
2. Download the Kaggle dataset and extract the CSV files (races.csv, drivers.csv, constructors.csv, etc.).
3. Open the .pbit Power BI Template in Power BI Desktop.
4. Connect the data source to the extracted CSV files or to a database of your choice.
5. Optionally, apply the included Power BI theme (.json) for consistent styling.
6. Refresh the data model to populate the visuals.

## References

Dataset: Formula 1 World Championship (1950–2020)
 by Rohan Rao

## License

This Power BI template is open for educational and personal use. Please credit the dataset author and this repository if you share or modify it.
