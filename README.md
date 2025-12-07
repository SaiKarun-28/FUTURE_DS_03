# College Event Feedback Analysis & Sentiment Classification

## 📌 Project Overview

This project analyzes student feedback collected from various college events (Tech Fest, Cultural Night, Hackathon, Sports Day). It combines quantitative data analysis (numerical ratings) with qualitative Natural Language Processing (Sentiment Analysis on text feedback) to derive actionable insights regarding student satisfaction.

The analysis is performed using **Python** in a Jupyter Notebook/Google Colab environment.

## 📂 Dataset Description

The analysis uses an Excel dataset (`College Feedback Sentiment-01.xlsx`) containing the following columns:

| Column | Description |
| :--- | :--- |
| **Student\_ID** | Unique identifier for the student |
| **Student\_Name** | Name of the student |
| **Department** | Student's academic department (CSE, ECE, IT, etc.) |
| **Year** | Year of study (1st, 2nd, 3rd, etc.) |
| **Event\_Name** | The event attended (e.g., Tech Fest, Hackathon) |
| **Feedback** | Textual feedback/review provided by the student |
| **Rating** | Numerical rating given (Scale: 1 to 5) |
| **Suggestions** | Specific suggestions for improvement |
| **Overall\_Experience** | Categorical rating (Excellent, Very Good, Good) |

## 🛠️ Tech Stack & Libraries

  * **Python**: Core programming language.
  * **Pandas**: Data manipulation, cleaning, and aggregation.
  * **Matplotlib & Seaborn**: Data visualization (Bar charts, Line plots).
  * **TextBlob**: Natural Language Processing (NLP) for sentiment polarity scoring.

## 📊 Key Analysis Steps

1.  **Data Preprocessing**:

      * Loaded the dataset and checked for duplicates.
      * Handled missing values in the `Suggestions` column (filled with "no opinion").
      * Verified data types and statistical summaries.

2.  **Exploratory Data Analysis (EDA)**:

      * Calculated the **Average Rating** per event.
      * Visualized ratings using Bar and Line charts to identify top-performing events.

3.  **Sentiment Analysis**:

      * Used **TextBlob** to generate a `Sentiment_Score` (Polarity) for each feedback entry.
          * *Polarity Range:* -1.0 (Negative) to 1.0 (Positive).
      * Classified sentiment into categories: **Positive**, **Neutral**, and **Negative**.
      * Aggregated sentiment scores by `Event_Name`.

## 📈 Key Findings

Based on the analysis performed in the notebook:

  * [cite_start]**Highest Rated Event:** `Tech Fest` (Avg Rating: 5.0)[cite: 110].
  * [cite_start]**Lowest Rated Event:** `Sports Day` (Avg Rating: 3.4)[cite: 110].
  * [cite_start]**Best Feedback Sentiment:** `Cultural Night` achieved the highest sentiment score (approx 0.42)[cite: 140], indicating highly positive verbal feedback despite having a lower numerical rating than Tech Fest.
  * [cite_start]**Worst Feedback Sentiment:** `Hackathon` had the lowest sentiment score (approx 0.29)[cite: 140], suggesting mixed feelings in the text reviews despite a decent numerical rating.
  * [cite_start]**Overall Sentiment:** The majority of feedback was **Positive** (16 counts), with minimal negative feedback[cite: 139].

## 🚀 How to Run

1.  **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/college-event-feedback-analysis.git
    ```
2.  **Install dependencies**:
    ```bash
    pip install pandas matplotlib seaborn textblob openpyxl
    ```
3.  **Run the Notebook**:
    Open `College Event Feedback Analysis.ipynb` in Jupyter Notebook or Google Colab.
4.  **Load Data**:
    Ensure the `College Feedback Sentiment-01.xlsx` file is in the root directory or update the file path in the code.

## 📷 Visualizations

The project generates the following visualizations:

  * [cite_start]**Bar Chart**: Average Rating by Event[cite: 112].
  * [cite_start]**Line Plot**: Trend of Ratings across events[cite: 112].
  * [cite_start]**Bar Chart**: Average Sentiment Score by Event[cite: 140].
  * [cite_start]**Count Plot**: Distribution of Sentiment Types (Positive/Neutral/Negative)[cite: 139].

-----
*Created by Sai Karun*
