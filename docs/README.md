
## Overview

This is a supporting website for the manuscript entitled **Simple Heuristics as a Viable Alternative to Machine Learning-based Anomaly Detection in Industrial IoT** submitted to the IEEE IoT Magazine. 

Our paper evaluates the efficacy of simple heuristic approaches compared to sophisticated machine learning by quantifying the accuracy and timeliness of selected multivariate anomaly detectors on industrial time series. It specifically examines the efficacy of two probabilistic detectors, a statistical detector and a deep learning anomaly detector. 

The presented work stems from the observation that the application of machine learning methods may be unfounded in a variety of use cases. 
The findings made in this study imply that there is no reason to over-engineer a solution by applying sophisticated methods without genuine grounds. 
The conventional autoregressive heuristic model outperforms the autoencoder by up to 7.2%. Furthermore, the autoencoder also underperforms in terms of execution time. Compared to the simpler approaches, its computational time complexity is up to 47% higher. 

Simple methods thus emerge as viable alternatives to sophisticated multivariate time-series anomaly detection on the evaluated application domain. 
Our conclusions remained valid through examining datasets originating from other domains. 
We infer that the performance of more elaborated methods requires verification to justify their usage.

## Insights

We examined the validity and generalizability of our findings using five datasets, all containing anomaly events.
 - SWAT represents a scaled-down version of a real-world, full-fledged, six-stage industrial water treatment plant producing five gallons per minute of water, containing anomaly events. 
 - MSL and SMAP are composed of telemetry data collected from two space missions. 
 - SKAB is an anomaly detection benchmark dataset containing industrial data from a water circulation system. 
 - Finally, SMD encompasses server machine-related data measured at a large internet company. 

In what follows, we provide inisghts into dataset characteristics[^1]. Each characteristics starts with a description, followed by the actual inisghts and concluded with a brief summary of findings.

[**SKAB**](html/SKAB.html) 

[**SMAP**](html/SMAP.html) 

[**SMD**](html/SMD.html) 

[**SWAT**](html/SWAT.html) 

[**MSL**](https://github-cloud.githubusercontent.com/alambic/media/514151638/1d/0a/1d0a025e67ad8cdeb26ed0d38ce4be598b23ffa66cfe6c4a413c6a75fd08a936?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIMWPLRQEC4XCWWPA%2F20221029%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20221029T180528Z&X-Amz-Expires=3600&X-Amz-Signature=060a1bef2958503586743e10a938b0ef79ad0b81005e3d22973a7f00e1a8abc9&X-Amz-SignedHeaders=host&actor_id=0&key_id=0&repo_id=557500842&token=1)

Upon close examination of the data distributions of these datasets, we observed a pattern that may be considered an indicator for algorithm selection. 
Heuristic algorithms seem to perform better on data sets of predominantly numerical features where the pairwise linear correlation between a subset of features is high. On the other hand, deep learning appears to extract complex anomaly patterns more efficiently in datasets where the categorical features are overrepresented. 
Uncovering hidden patterns and relationships within the datasets can certainly help determine actionable steps to maximize anomaly detection efficacy. 
However, further study is needed to develop systematic methodology selection strategies operating reliably in a wide variety of use cases.

[^1]: Please let us know if any links are unavailable via a repository issue.
