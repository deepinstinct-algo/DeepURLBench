# DeepURLBench Dataset

This repository contains the dataset **DeepURLBench**, introduced in the paper **"A New Dataset and Methodology for Malicious URL Classification"** by Deep Instinct's research team.

## Dataset Overview

The repository includes two parquet directories:

1. **`urls_with_dns`**:
   - Contains the following fields:
     - `url`: The URL being analyzed.
     - `first_seen`: The timestamp when the URL was first observed.
     - `TTL` (Time to Live): The time-to-live value of the DNS record.
     - `label`: Indicates whether the URL is malware, phishing or benign.
     - `IP addresses`: The associated IP addresses.

2. **`urls_without_dns`**:
   - Contains the following fields:
     - `url`: The URL being analyzed.
     - `first_seen`: The timestamp when the URL was first observed.
     - `label`: Indicates whether the URL is malware, phishing or benign.

## Usage Instructions

To load the dataset using Python and Pandas, follow these steps:

```python
import pandas as pd

# Replace 'directory' with the path to the parquet file or directory
df = pd.DataFrame.from_parquet("directory")

## License

This dataset is licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/). You are free to use, share, and adapt the dataset for non-commercial purposes, with proper attribution.
