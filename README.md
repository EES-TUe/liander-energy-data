# liander-energy-data

Experimental helper script for Liander Open Energy Data.

## Background

LianderPower is an open dataset containing anonymized historical time series data from Liander's electricity distribution network, covering the period 2013–2024 with 5-minute interval measurements and historical weather information. The dataset is designed for research in time series modeling, forecasting, imputation, and machine learning applications for electricity networks. All data has been carefully anonymized and aggregated to protect privacy, with locations obscured through random spatial jittering within 5 km and no sensitive information such as customer data, exact asset locations, or network topology included. The dataset is available in Parquet format with Croissant metadata and is published under the Creative Commons Attribution 4.0 International (CC BY 4.0) license.

### Dataset Information

| Item | Value |
|------|-------|
| Publisher / creator | Alliander / Liander |
| Maintainer | System Operations AI R&D team, Alliander |
| Substantive owner / contact | Jessica Loke, Research & Innovation Specialist, System Operations, Alliander; [jessica.loke@alliander.com](mailto:jessica.loke@alliander.com) |
| License | Creative Commons Attribution 4.0 International (CC BY 4.0) |
| Refresh frequency | Intended annual refresh, subject to data-governance review |
| Measurement cadence | 5 minutes (300 seconds) |
| Weather cadence | 1 hour (3,600 seconds), UTC |
| Geographic scope | Liander service area in the Netherlands; public coordinates are anonymized/jittered |


## Getting Started

### 1. Install uv

If you don't already have `uv` installed, follow the [official uv installation guide](https://docs.astral.sh/uv/getting-started/installation/).

### 2. Clone the repository and sync dependencies

```bash
git clone https://github.com/EES-TUe/liander-energy-data.git
cd liander-energy-data
uv sync
```

### 3. Open in VS Code and run the notebook

1. Open the folder in VS Code:
   ```bash
   code .
   ```
2. Open the Jupyter notebook (`liander-energy-data.ipynb`)

### 4. Download the data

The data files are available from Liander's open data portal:
- Visit https://www.liander.nl/over-ons/open-data
- Navigate to the **LianderPower** section
- Download the ZIP file
- Unzip the downloaded file
- Extract the `data` folder from the ZIP file into the repository root `data/` directory

## License

This experimental script is licensed under the **BSD 3-Clause License**. See the [LICENSE](LICENSE) file for details.

The **LianderPower dataset** that you download is published under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license. When using the data, you must provide appropriate attribution to Liander.
