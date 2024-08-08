# RevStream-InsightFlow: An end-to-end data pipeline on GCP
RevStream InsightFlow is a data pipeline leveraging the 2023 Amazon Reviews dataset to extract, transform, and analyze user reviews. The project offers insights into customer sentiment, product performance, and user engagement using GCP services like BigQuery, Dataproc, and Looker Studio.
## Dataset

The dataset used in this project is the [Amazon Reviews 2023](https://www.kaggle.com/datasets/wajahat1064/amazon-reviews-data-2023). It includes:

- **User Reviews**: Ratings, review text, helpfulness votes, and more.
- **Item Metadata**: Product descriptions, pricing, images, and more.
### Key Features of the Dataset:

- **Larger Dataset**: 571.54M reviews, 245.2% larger than previous versions.
- **Richer Metadata**: Descriptive item features.
- **Fine-grained Timestamp**: Interaction timestamp at the second or finer level.

## Tech Stack

- **Data Storage**: [Google Cloud Storage (GCS)](https://cloud.google.com/storage)
- **Data Processing**: [Dataproc](https://cloud.google.com/dataproc)
- **Data Transformations**: [Data Build Tool (DBT)](https://www.getdbt.com/)
- **Data Warehouse**: [BigQuery](https://cloud.google.com/bigquery)
- **Workflow Orchestration**: [Cloud Composer](https://cloud.google.com/composer)
- **Programming Language**: [Python](https://www.python.org/)
- **Infrastructure as Code**: [Terraform](https://www.terraform.io/)
- **Data Visualization**: [Google Data Studio](https://datastudio.google.com/)
- **CI/CD**: [Cloud Build](https://cloud.google.com/build), [Cloud Run](https://cloud.google.com/run)

## Pipeline Overview

The pipeline includes the following steps:

1. **Data Loading**: Loading the Amazon Reviews dataset using Huggingface's `datasets` library.
2. **Data Processing**: Cleaning and transforming the data using GCP's Dataproc and BigQuery.
3. **Data Analysis**: Performing exploratory data analysis (EDA) to identify trends and insights using DBT and BigQuery.
4. **Data Visualization**: Creating interactive dashboards using Google Data Studio to visualize insights.
5. **Orchestration**: Using Cloud Composer to orchestrate various steps of the pipeline.
6. **CI/CD**: Dockerizing DBT jobs and deploying them using Cloud Build and Cloud Run.

## Pre-Requisites

- **Operating System**: Linux Preferred
- **Tools**: Python, Terraform, Git
- **GCP Resources**: A GCP Project, service account and GCloud CLI

## Setting up the Pipeline
I've written a detailed blog with steps to recreate this pipeline. You can visit the blog [here]() and follow the steps
## Dashboard
The final dataset, processed and stored in BigQuery, is used to create a dashboard using Google Data Studio. This dashboard provides:

- **Customer Sentiment Analysis**: Visual representations of positive, neutral, and negative sentiments in reviews.
- **Product Performance Insights**: Key metrics like average ratings, most reviewed products, and more.
- **User Engagement Patterns**: Trends in user interaction, review frequency, and more.

## Conclusion
RevStream InsightFlow provides a scalable and efficient way to analyze Amazon reviews and gain actionable insights. The project can be extended with additional features such as sentiment analysis, trend analysis, and customer segmentation.

Feel free to explore, use, and contribute to this project!

