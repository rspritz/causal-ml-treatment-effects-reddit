# causal-ml-treatment-effects-reddit
This project uses Double Machine Learning (DML) and Causal Forest methods to show that during COVID-19, in mainstream subreddits, partisan language decreased user engagement with posts. These results suggest that there is a polarization penalty for online content. [Read the full paper (PDF)](The%20Polarization%20Penalty_Partisan%20Intense%20Language%20and%20Online%20Engagement_Rebecca%20Spritzer.pdf)

The main script to run is ANALYSIS_CODE. This notebook utilizes reddit_datset_final_politicaladded.parquet which includes political classifications generated using the alhalla/distilbart-mnli-12-3 model.

Since Large Languag eModels(LLMs) can exhibit stochastic variation this script is designed to load the pre-computed labels to ensure exact replication of the results presented in the paper.

If interested in the label classification, the source logic is available upon request [rebecca.spritzer@gmail.com]. Re-running the classification will yield marginally different labels but will not significantly alter the direction or significance of the average treatment effect.
