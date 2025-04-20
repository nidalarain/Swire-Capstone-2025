# Swire Coca-Cola Capstone Project

This repository contains my individual work for the Swire Coca-Cola Capstone Project, part of the MSBA program at the University of Utah. The goal of this project was to help Swire optimize its delivery operations by identifying which customers could be transitioned to a more cost-efficient delivery method (white trucks) without sacrificing long-term growth potential.

## Business Problem & Objective

Swire Coca-Cola incurs high logistics costs servicing low-volume customers with its own fleet (red trucks). While moving some of these customers to third-party (white truck) delivery could reduce costs, doing so prematurely for high-growth customers may hinder future revenue. The objective was to identify which customers could be rerouted without hurting growth, and which should remain on red trucks due to strong volume or growth potential.

## Our Team's Solution

Our team used a multi-pronged modeling approach:
- RFM segmentation to engineer relevant behavioral features
- K-Means clustering to group customers into volume-based segments
- Random Forest and Decision Tree models to identify key predictors of volume and growth
- ARIMA forecasting to project channel-level growth
- Scoring system to rank customers by growth potential based on economic and order data
We then developed routing rules that leveraged these insights to assign customers to red or white trucks based on volume thresholds, growth potential, and order frequency.

 ## My Contribution

My primary focus was on the clustering and predictive modeling components:
- Led the creation of behavioral features using RFM (Recency, Frequency, Monetary Value)
- Ran PCA and K-Means clustering to segment customers into distinct profiles
- Built a Random Forest model to validate cluster separation and identify important drivers
- Developed a growth potential score using normalized economic and order variables
- Proposed new fleet assignment rules combining volume, growth signals, and clustering insights

## Business Value

The results of our modeling allowed Swire to:
- Reduce delivery costs by confidently rerouting true low-volume, low-growth customers
- Preserve high-touch service for customers showing strong potential, even if current volume was low
- Establish a repeatable framework for fleet assignment using scalable business rules and growth analytics

## Challenges Along the Way

The initial project scope was broad, and the first sponsor presentation wasn't recorded, making it difficult to revisit requirements early on
Data integration required a lot of cleanup, especially merging customer, transaction, and ZIP-level census data
Balancing cost savings with long-term customer potential was a nuanced business problem that required both technical modeling and domain insight

## What I Learned

- How to apply clustering and supervised modeling to a real-world logistics challenge
- Importance of feature engineering in aligning data with business goals
- Communicating technical results in a way that business leaders can act on
- How to use public census data to enrich customer insights

This project not only helped me build technical skills but also gave me experience in navigating an ambiguous business problem and producing actionable insights.

Thanks for reading! Check out my individual notebooks for:

Swire_EDA.rmd — Exploratory data analysis and feature engineering

Swire Capstone Modeling.rmd — Clustering, Random Forest model, and growth scoring

