# Changepoint Analysis

This repository includes an R Markdown file (`Changepoint.Rmd`) that performs changepoint analysis on a dataset (`UBHPC_8cores_NWChem_Wall_Clock_Time.csv`) representing runtime data for a computational task. The analysis aims to identify segments in the data where there are significant changes in magnitude or trend patterns.

## Files

1. **Changepoint.Rmd**: R Markdown file containing the code for changepoint analysis. The analysis is conducted on the `UBHPC_8cores_NWChem_Wall_Clock_Time.csv` dataset.

2. **Homework_5.knit.pdf**: Compiled PDF document generated from the R Markdown file, providing a detailed explanation of the changepoint analysis, methodology, and results.

## Dataset

The dataset (`UBHPC_8cores_NWChem_Wall_Clock_Time.csv`) consists of runtime data with corresponding dates. The goal is to identify and analyze segments within the data where there are significant changes in the runtime behavior.

## Changepoint Identification

The analysis involves the following steps:

1. **Visual Identification of Segments:** The code visually identifies four segments in the runtime data based on changes in magnitude and trend patterns.

2. **Segmentation:** The identified changepoints are used to segment the data into distinct periods, each characterized by its own behavior.

3. **Distribution Analysis:** The code generates histograms and QQ plots for each segment to assess the normality of the data within each segment.

4. **Changepoint Detection Algorithms:** Two changepoint detection algorithms (`cpt.meanvar` and `cpt.var`) are employed to automatically identify changepoints in the data.

5. **Optimal Number of Segments:** The code uses the CROPS (Cost-complexity Ranking for Online Profile Segmentation) algorithm to determine the optimal number of segments, which may differ from the initial visual estimate.

6. **Visualization:** The identified changepoints and segmented data are visualized using line plots, histograms, and QQ plots.

## Conclusion

The changepoint analysis provides insights into the dynamics of the runtime data, helping to identify periods with distinct characteristics. It emphasizes the importance of data-driven decision-making, especially when choosing the number of segments and optimizing changepoint detection.

It is crucial to note that the normality assumption in the initial analysis is challenged, and alternative approaches may be necessary for more accurate changepoint identification. Consideration of the actual distribution of the data is recommended for robust analysis and decision-making.

