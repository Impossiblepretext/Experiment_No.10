# Experiment – 10
## Title

Creation, Storage, and Loading of Datasets using Pandas

## Aim

To study the process of manual dataset creation in Python and understand the methodologies for loading, exporting, and performing initial structural analysis on external data files.

## Objectives
 
To learn how to construct a DataFrame from raw Python dictionaries
To explore various file export formats including CSV and Excel
To understand the mechanisms for loading external datasets from local and cloud directories
To perform basic structural inspection using shape, size, and metadata attributes
To implement data selection and filtering techniques (loc, iloc, and column-based access)
To apply basic descriptive statistical functions and schema modification methods

## Theory on Dataset Management

In the lifecycle of Exploratory Data Analysis (EDA), data management begins with either manual creation for testing purposes or, more commonly, loading large-scale datasets from external sources. Pandas provides a robust framework for handling these transitions through its specialized input/output (I/O) API.

### 1. Manual Dataset Construction

Data can be structured in Python using dictionaries where keys represent column headers and values (lists) represent the data rows. By passing these structures into a DataFrame constructor, Pandas creates a tabular representation that supports relational operations. This is vital for creating dummy data or small-scale look-up tables.

### 2. Data Persistence (Exporting)

Once a dataset is created or modified in the memory (RAM), it must be saved to permanent storage to be shared or used later.

CSV (Comma Separated Values): A lightweight, plain-text format that is universally accepted across data platforms.
Excel (.xlsx): A binary format that supports multiple sheets and complex formatting, often used in business environments.

## Structural Inspection Theory

Before analyzing data, a researcher must understand its structure. Pandas provides several attributes for this:

Shape: Returns a tuple representing the dimensionality (Rows, Columns).
Size: Represents the total number of elements (Rows × Columns).
Info(): Displays the DataFrame's schema, including column names, non-null counts, and memory usage.
Dtypes: Each column is assigned a specific data type (int64, float64, object/string). Understanding these types prevents logical errors.

## Data Retrieval and Modification
### 1. Accessing Observations

Data can be retrieved through two primary methods:

Label-based Selection: Using column names or .loc to access rows based on index labels.
Position-based Selection: Using .iloc to access data based on numerical position.

### 2. Slicing the Dataset

To avoid loading all rows at once when working with large datasets, head() and tail() functions are used.
head() shows the first few rows, while tail() displays the last few rows.

### 3. Dynamic Schema Modification

A dataset may require changes after loading. Pandas allows:

Column Addition: Adding new columns derived from existing data.
Column Dropping: Removing unnecessary columns.
Aggregate Functions: Using functions like min() and max() to analyze numerical columns.

## Applications in Engineering

Sensor Data Logging: Structuring real-time sensor readings into datasets.
Network Analysis: Loading and analyzing server log files.
Market Analysis: Comparing hardware specifications and pricing data.

## Conclusion

The ability to create, save, and reload datasets forms the foundation of data analysis. By understanding Pandas I/O operations and structural attributes, we can efficiently manage datasets and prepare them for deeper analytical processing.
