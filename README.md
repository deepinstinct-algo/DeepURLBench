# DeepURLBench Dataset

This repository contains the dataset **DeepURLBench** for the paper:  
**"A New Dataset and Methodology for Malicious URL Classification"**  
by Deep Instinct's Research Team.

---

## Dataset Description

The repository includes two directories in Parquet format:

1. **`urls_with_dns`**: Contains URLs with associated DNS data.
2. **`urls_without_dns`**: Contains URLs without DNS data.

---

## Loading the Dataset

You can load the dataset using **pandas** in Python. Here's an example:

```python
import pandas as pd

# Load a Parquet file
df = pd.read_parquet('path_to_directory')
