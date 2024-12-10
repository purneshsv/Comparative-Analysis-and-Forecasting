# Comparative Analysis and Forecasting of GitHub Repository Metrics Using Advanced Time Series Models

## Overview
This project focuses on monitoring GitHub repository metrics, including the number of issues created and resolved over the past two years, and predicting future trends using advanced time series models. The project also includes deploying data to Google Cloud.

---

## GitHub Repositories Analyzed:
1. [Langchain](https://github.com/langchain-ai/langchain)
2. [Langgraph](https://github.com/langchain-ai/langgraph)
3. [Autogen](https://github.com/microsoft/autogen)
4. [OpenAI Cookbook](https://github.com/openai/openai-cookbook)
5. [Elasticsearch](https://github.com/elastic/elasticsearch)
6. [Pymilvus](https://github.com/milvus-io/pymilvus/)

---

## Part I: Time Series Forecasting Models
### Models Utilized:
1. **Long Short-Term Memory (LSTM)**
   - Designed to address the vanishing gradient problem.
   - Captures intricate dependencies in sequential data.
   - Used in tasks such as speech recognition, time series forecasting, and natural language processing.

2. **Facebook Prophet**
   - Open-source forecasting tool by Facebook’s Core Data Science team.
   - Handles seasonality and events automatically.
   - Suitable for fast, accurate time series forecasting.

3. **Statsmodel**
   - Python library for statistical modeling and hypothesis testing.
   - Includes tools for linear regression, generalized linear models, and time series analysis.

### Performance Comparison:
- **Best Performing Model:** Facebook Prophet
- **Least Performing Model:** Statsmodel

---

## Part II: Data Retrieval and Analysis
### Data Retrieval:
- Data was fetched from GitHub repositories for the last two months using Python and the GitHub API.
- Created vector embeddings for issues and stored them in Elasticsearch.

### Analysis:
Performed the following tasks using `Analytics.ipynb`:
1. **Bar Chart Analysis:**
   - Analyzed the number of issues created each day of the week across repositories.

2. **Semantic Search with Vector Embeddings:**
   - Ranked issues by similarity scores.
   - Identified the top five comparable issues per repository.

---

## Key Insights
- **Time Series Insights:** Trends in issue creation and resolution using TensorFlow LSTM, Facebook Prophet, and Statsmodel.
- **Semantic Search:** Enhanced issue identification and comparison using Elasticsearch and vector embeddings.

---

## Visualizations
### Metrics Covered:
- Created vs. Closed Issues
- Weekly and Monthly Issue Trends
- Maximum Issues by Day of the Week
- Time Series Forecasting for:
  - Issues Created
  - Issues Closed
  - Pull Requests
  - Commits

### Example Charts:
- Bar charts for daily issue trends.
- Line graphs for time series forecasts.

---

## Deployment
- Data and results were deployed to Google Cloud for further analysis and scalability.

---

## Project Structure
- `Part1/`: Scripts for data retrieval and forecasting.
- `Part2/`: Elasticsearch integration and semantic search implementation.
- `Analytics.ipynb`: Notebook containing data analysis and visualizations.

---

## Tools and Technologies
- **Programming Language:** Python
- **Libraries and Frameworks:** TensorFlow, Keras, Statsmodel, Facebook Prophet
- **Database:** Elasticsearch
- **Cloud Platform:** Google Cloud

---

## Author
**Purnesh Shivarudrappa Vidhyadhara**  
Master’s Student, Computer Science   
Illinois Institute of Technology  


---

## Acknowledgments
- GitHub API for data retrieval.
- TensorFlow, Keras, Facebook Prophet, and Statsmodel for time series analysis.
- Elasticsearch for advanced search and embedding-based similarity analysis.
