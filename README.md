# Marketing Campaign Performance Analysis using AI

## Project Overview
**Project Title:** Marketing Campaign Performance Analysis using AI  
**Role:** Data Science Intern  

This project aims to develop an AI-powered system that analyzes marketing campaign performance, generates insights, and provides data-driven recommendations to optimize marketing strategies.

## Objective
The goal of this project is to leverage AI for analyzing marketing campaign data, extracting key insights, and improving decision-making for marketing teams.

## Features
- **Retrieval-Augmented Generation (RAG) System:** Enables efficient data retrieval and insight generation.
- **NLP-Powered Insights:** Uses Google Gemini for natural language processing.
- **Similarity Search:** Implements Sentence Transformers and FAISS for fast and accurate search.
- **Key Metrics Analysis:** Examines revenue, click-through rates, conversion rates, and campaign effectiveness.
- **Automated Summary Reports:** Generates reports with essential marketing KPIs.

## Technologies Used
| Technology | Purpose |
|------------|---------|
| Python (Pandas, NumPy) | Data processing & analysis |
| Google Gemini (Generative AI) | AI-powered insights generation |
| Sentence Transformers (all-MiniLM-L6-v2) | Text embeddings for semantic search |
| FAISS (Facebook AI Similarity Search) | Efficient vector similarity search |
| Google Colab / Jupyter Notebook | Development environment |

## Workflow & Implementation
### Step 1: Data Preparation
- Loaded and pre-processed CSV data (`updated_dataset.csv`).
- Extracted date-related features such as day, month, and quarter.
- Created a combined text field for embedding generation.

### Step 2: Embedding Generation
- Used **Sentence Transformers (all-MiniLM-L6-v2)** to generate embeddings.
- Stored embeddings in a FAISS index for fast similarity search.

### Step 3: Query Processing & RAG Integration
- Converted user queries into embeddings.
- Retrieved the top-5 most similar records using FAISS.
- Provided context to **Google Gemini** for detailed analysis.

### Step 4: AI-Powered Analytics
- Generated insights including:
  - Direct answers to queries.
  - Key campaign performance insights.
  - Trend analysis and recommendations.

### Step 5: Summary Report Generation
- Generated key performance metrics, including:
  - Total revenue
  - Average click-through rate (CTR%)
  - Total leads
  - Best-performing campaigns

## Key Findings & Insights
- **Highest Revenue Campaign:** `B2C_RSB_MPN_DIRECTBL_17juneAP1_Propensity` generated the highest revenue ($103.99).
- **Best Conversion Rate Channel:** SMS had the highest click-to-lead conversion rate (9.9%).
- **Top Lead Generation Campaign:** `DPPM_BL_OB_DPDM_SMS1` generated the most leads (72).
- **Revenue Trends:** June 2024 had higher revenue than November 2024.
- **Underperforming Campaigns:** Some campaigns generated $0 revenue and should be optimized.

## Challenges Faced
- **Limited Data:** Only two months of data were available, limiting trend analysis.
- **Missing Cost Data:** ROI calculations were not possible due to missing cost metrics.
- **Seasonal Pattern Detection:** More historical data is needed for accurate trend identification.

## Future Work & Recommendations
✅ Expand the dataset to include more months/years for better trend analysis.  
✅ Incorporate cost-per-impression data to calculate ROI.  
✅ Implement A/B testing for campaign strategy optimization.  
✅ Conduct customer segmentation to analyze performance based on demographics.  
✅ Develop real-time analytics for live campaign monitoring.  

## Conclusion
This project successfully built an AI-driven marketing analytics system using **Google Gemini**, **Sentence Transformers**, and **FAISS**. It provided actionable insights that can improve marketing campaign efficiency and revenue generation. Future enhancements could include **predictive modeling** for campaign forecasting and **automated report generation** for stakeholders.

## Installation & Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/marketing-ai-analysis.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter Notebook:
   ```bash
   jupyter notebook Gemini.ipynb
   ```

## License
This project is licensed under the [MIT License](LICENSE).

## Author
**Ashutosh Kumar**  
Email: mailtooashu321@gmail.com  

---
Feel free to update the repository links and additional details as needed!

