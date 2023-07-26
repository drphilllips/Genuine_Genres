# Genuine_Genres

Spring, 2023,
SOLO PROJECT for WPI Graduate Course, CS 539: Machine Learning

The original goal of this project was to train a Clustering Algorithm on
Spotify Audio features (X) for songs by track genre (y) to be able to create
an accurate prediction of genre based purely on audio features.
       **this hypothesis was inspired by the fact that Spotify has uniquely measured audio features
         including danceability, liveness, valence, energy, and much more

After months of research and revising the model, I realised it wasn't the success of the model
that was important, but rather the approach to clustering and specifically, dimensionality reduction.

The following abstract is from my final, written report...

## Abstract

Through the development of a new pre-processing step for cluster analysis and the results of test and control models, this project validates the proposed clusterability metric to be used for feature selection. This project goes through the several data collection and reduction steps that worked to create a new dataset containing advanced Spotify audio features over 180,000 songs across 1,200 unique genres, as well as the analysis of that dataset which verifies the improvement in models with clusterability-selected features. The clusterability metric is similar to the Calinski Harabasz index (Calinski & Harabasz, 1974) in that it measures intra-variance to inter-variance of groups; however, because it is used in the preprocessing stage, it is a novel application of the concept. The base clustering model of choice was k-nearest neighbors. The test model was fitted with only those features achieving a clusterability score above 1.0, and the control was fitted with all features. The main evaluation metrics used to compare models were the Calinski Harabasz index, silhouette score, the Davies Bouldin index, and normalized mutual information. The outcome of the various tests on each model showed that out of 14 test scenarios with significant differences in performance, the clusterability feature-selected model outperformed the control model in 13 of them. With these results the outcome of this paper is that there is hopefully more research done to either validate this preprocessing step, or to specify in which scenarios it performs best.

Keywords: machine learning, k-nearest neighbors, clustering, dimensionality reduction, Spotify audio features

## Table of Contents

- README.md
{ project_phillips
       - Written Report.docx : Final written report and summary of the project
       { results
              - process_notebook.ipynb : Process explanations and code for all findings

