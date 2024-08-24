# COVID-19 Time Series Visualization and Clustering

This project focuses on visualizing and clustering COVID-19 time series data to uncover patterns and insights across different regions. Utilizing data from Johns Hopkins University, this analysis aims to enhance understanding of the pandemic's dynamics through data visualization and advanced clustering techniques.

## Table of Contents

- [Overview](#overview)
- [Objectives](#objectives)
- [Methodology](#methodology)
  - [Data Collection](#data-collection)
  - [Data Preprocessing](#data-preprocessing)
  - [Visualization](#visualization)
  - [Clustering Analysis](#clustering-analysis)
  - [Pattern Exploration](#pattern-exploration)
  - [Anomaly Detection](#anomaly-detection)
- [Results](#results)
  - [Visualizations](#visualizations)
  - [Cluster Identification](#cluster-identification)
  - [Pattern Recognition](#pattern-recognition)
- [Evaluation of Clustering](#evaluation-of-clustering)
- [Skills Demonstrated](#skills-demonstrated)
- [Conclusion](#conclusion)
- [Visuals and Results](#visuals-and-results)
- [Contact](#contact)

## Overview

The COVID-19 pandemic has significantly impacted global health, economies, and social structures. Analyzing its progression through data-driven approaches can provide valuable insights for policymakers and health professionals. This project employs my analytical skills and expertise in data science to explore COVID-19 time series data, offering a detailed examination of regional trends and patterns.

## Objectives

- **Visualization:** Create interactive and intuitive visualizations of COVID-19 cases, recoveries, and deaths using Plotly.
- **Clustering:** Use clustering algorithms to identify regions with similar pandemic trends and dynamics.
- **Pattern Recognition:** Analyze time series data to detect significant patterns and correlations.
- **Data Insights:** Provide actionable insights that can inform public health decisions and strategies.

## Methodology

1. **Data Collection:** Data was sourced from the comprehensive datasets provided by Johns Hopkins University, which includes daily reports of COVID-19 statistics worldwide.
   
2. **Data Preprocessing:** The data was cleaned and organized to ensure accuracy and consistency for analysis.

3. **Visualization:** Leveraging Plotly, the project creates interactive charts and visualizations to effectively communicate trends in COVID-19 data, highlighting key metrics across different regions.

4. **Clustering Analysis:** Applying clustering algorithms, such as K-Means, to identify regions with similar pandemic behaviors and group them effectively.

5. **Pattern Exploration:** Conducting exploratory data analysis (EDA) to identify underlying patterns and trends in the time series data.

6. **Anomaly Detection:** 
   - **Algorithm Explanation:**
     1. **Calculate Slope:** The algorithm calculates the slope between two points in the time series. Each point is defined by its timestamp and value. The slope is computed as the change in value divided by the change in time (in seconds).
     2. **Check for Anomalies:** For each country, the algorithm calculates slopes between points separated by a given period. It then scales these slopes to a range of [-1, 1] using MinMaxScaler. If the slope is below a certain threshold, it is considered significant. The slopes are checked for anomalies based on their scaled values.
     3. **Determine Longest Sequence of Anomalies:** The algorithm converts the list of slopes into binary values (1 if the slope is below the threshold, otherwise 0). It then finds the longest consecutive sequence of 1s (which represent anomalies).
     4. **Update Anomaly DataFrame:** If the longest sequence of anomalies for a country is greater than or equal to a specified length (e.g., 390), the country is flagged as an anomaly and included in the final results.

## Results

- **Visualizations:** Interactive charts and visualizations created with Plotly provide an engaging way to explore COVID-19 trends and impacts across various regions.
  
- **Cluster Identification:** The clustering analysis successfully identifies regions with similar pandemic trajectories, enabling targeted insights.

- **Pattern Recognition:** The analysis uncovers significant patterns in COVID-19 data, highlighting correlations that can aid in understanding the pandemic's dynamics.

## Evaluation of Clustering

**Evaluating Clustering for Original Clustering:**
- **WCSS for Original Clustering:** 5444.1308416424304
- **Silhouette Score for Original Clustering:** -0.0575844975399092
- **Davies-Bouldin Index for Original Clustering:** 2.0677513509480425
- **Calinski-Harabasz Index for Original Clustering:** 13.92327688635464

**Evaluating Clustering for Improved Clustering:**
- **WCSS for Improved Clustering:** 3583.278671689847
- **Silhouette Score for Improved Clustering:** 0.10887256392207167
- **Davies-Bouldin Index for Improved Clustering:** 1.9982249277911357
- **Calinski-Harabasz Index for Improved Clustering:** 15.328455771236404

![Evaluation](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEiTo5ttHgQAUasCh6svzeyfW2GqovpfT5XRVFYbMjpF7kriiGAQDm6VcmKicEI37klk3hGRHkFCqGknvco9tHirzmM1fAf7gWw5kjr35bI9krflN6Dne6qZxocMFW-4sLPvUNmePCGE9f24RM859NaHGOVKHZ2Vc5SPwxp4I0pZ0Q_ffxfr_wjnKq5is5E/s1600/evaluation.png)

## Skills Demonstrated

- **Data Analysis:** Proficient in analyzing complex datasets and extracting meaningful insights.
- **Data Visualization:** Skilled in creating interactive visualizations using Plotly that effectively communicate data-driven stories.
- **Machine Learning:** Experienced in applying clustering algorithms to identify patterns in time series data.
- **Problem-Solving:** Demonstrated ability to employ analytical thinking to solve complex problems and provide actionable insights.

## Conclusion

This project showcases my ability to apply data science techniques to real-world challenges, demonstrating my skills in analytical thinking, problem-solving, and interactive data visualization. By exploring COVID-19 time series data, the project contributes to the broader understanding of the pandemic and provides valuable insights for public health strategies.

## Visuals and Results

![COVID-19 Clusters](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhOzhn9mNdfu24peG5r2bR90EkHroeGeuBSGeSnyZ4s3v8p6N38tlOcDW1XIL5j4m16qz-SZKNiDF-3XXRGp2y5cFGz2jbb_xxEG4uJFwu2umN0LBD73BAFvQSNw983YqlsSthqy4iqkootTq9lGZbAfSCi0jn3rP90pWBJuM57q4zw9pwdtcQV43iR5qg/s1600/clusters.png)  
![World Map](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgiaNFJs_9krCIOe8mefoTI8VJB3422RrqBBvXexyO-23Zq9EiUNFo25tLtEgTeHb-D4KkRmUybPRNE_LdbbJ-kgchPA0049q5J62L4gKXs1Nwbi0X41O_XgiSFJwrmKCvm0Gr38xSNIbVvz5Eb3GxP8aC9qUlFyosISOnCX5_0qLHLcV1LaA_pcgdUehk/s1600/WorldMap%20with%20Clusters.png)


## Google Colab

You can view and run the notebook directly on [Google Colab](https://colab.research.google.com/drive/1kmQf86LpNGwQrsAvgpzsAfhn-MCUuHVW?usp=sharing).

Feel free to explore the project files and code to gain deeper insights into the analysis and findings. Your feedback and contributions are welcome!

## Contact

**Ahmed Atta Ramadan**  
[ahmedatia456123@gmail.com](mailto:ahmedatia456123@gmail.com)
