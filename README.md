# HIV Study Analysis and Visualization

This repository contains R scripts for analyzing and visualizing the geographic and temporal distribution of HIV studies. The analysis incorporates data manipulation, statistical computations, and the generation of visualizations using various R libraries.

---

## Specific Aims

The goal of this study is to enhance the understanding of HIV research distribution across geographic regions, income groups, and study focus areas. The specific aims are as follows:

1. **Aim 1: Geographic and Temporal Analysis of HIV Studies**
   - Assess the global distribution of HIV studies over time and across geographic regions.
   - Identify trends in HIV research by analyzing study prevalence in high-income, middle-income, and low-income countries.

2. **Aim 2: Analysis of Tissue Sources and Study Focus**
   - Investigate the representation of tissue specimen sources in HIV studies (e.g., "blood" vs. "other") and the extent of missing or unspecified data.
   - Compare the prevalence of research on envelope proteins versus other proteins in HIV studies across different countries and income groups.

3. **Aim 3: Visualization and Dissemination of Findings**
   - Develop intuitive visualizations, including maps, bar charts, and pie charts, to communicate the study findings effectively.
   - Highlight disparities in research focus and distribution to inform future HIV research funding and resource allocation.

---

## Features

1. **Data Cleaning and Transformation**
   - Replaces missing or ambiguous country data with appropriate labels.
   - Harmonizes country names for compatibility with geographic datasets.

2. **Geographic Distribution Analysis**
   - Merges HIV study data with Natural Earth's geographic data.
   - Generates static and interactive maps to display the number of HIV studies by country.

3. **Temporal Distribution Analysis**
   - Aggregates HIV cases by predefined time periods.
   - Creates bar charts showing case distributions over time.

4. **Income Group Analysis**
   - Combines countries into broader income categories for analysis.
   - Produces box plots, bar charts, and pie charts to explore relationships between income groups and study counts.
   - Highlights top contributing countries in each income group.

5. **Tissue and Protein Study Analysis** *(New)*
   - Examines the prevalence of different tissue specimen sources (e.g., "blood" vs. "other").
   - Identifies and visualizes the percentage of missing or unspecified data across income groups.
   - Compares envelope proteins to all proteins in HIV studies by country and income group.

6. **Summary Statistics**
   - Calculates summary statistics for each income group (mean, median, standard deviation, etc.).
   - Displays the percentage of studies contributed by top countries.

---

## Visualizations

The repository generates the following key visualizations:

1. **Bar Chart**: Distribution of HIV cases over 5-year intervals.
2. **Static Map**: Global distribution of HIV studies by country.
3. **Box Plot**: Study counts by income group.
4. **Stacked Bar Chart**: Top contributing countries for each income group.
5. **Pie Charts**: Proportions of studies by country within income groups.
6. **Tissue Specimen Bar Chart** *(New)*: Comparison of "blood" vs. "other" tissue sources.
7. **Missing Data Bar Chart** *(New)*: Percentage of unspecified tissue sources by income group.
8. **Protein Study Bar Chart** *(New)*: Comparison of envelope proteins vs all proteins by income group.

---

## Requirements

- **R (version >= 4.0)**
- **R packages**:
  - `tmap`
  - `sf`
  - `rnaturalearth`
  - `rnaturalearthdata`
  - `dplyr`
  - `ggplot2`
  - `lubridate`
  - `tidyr`
  - `car`

---

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```

2. Install the required R packages:
   ```R
   install.packages(c("tmap", "sf", "rnaturalearth", "rnaturalearthdata", "dplyr", "ggplot2", "lubridate", "tidyr", "car"))
   ```

3. Open the R scripts in your preferred IDE (e.g., RStudio).

4. Ensure your dataset includes the required columns (e.g., `Country`, `Tissue_Specimen_Source`, `income_grp_combined`, `protein_length`).

5. Execute the scripts to:
   - Perform data cleaning.
   - Generate analyses.
   - Create visualizations saved in the output directory.

---

## Example Outputs

1. **Temporal Distribution**: `5yr_hiv_cases_by_counts.png`
2. **Geographic Distribution**: `hiv_distribution_map.png`
3. **Income Group Analysis**: `a.1.2.income_dist.pdf`
4. **Tissue Specimen Analysis**: `IO2.3.pdf`, `IO2.pdf`
5. **Protein Study Analysis**: `Aim2.1.a.png`

---

## Data Source

- The geographic data is sourced from the [Natural Earth](https://www.naturalearthdata.com/) dataset.

---

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

## Contributions

Contributions are welcome! Feel free to submit issues or pull requests for improvements or additional features.

---
