# 📺 YouTube Trending Video Analysis

## 🧠 Project Overview  
This project explores over 100,000 YouTube trending videos across multiple countries to uncover patterns in content performance, audience engagement, and channel behavior. Using Python, SQL, and machine learning, it builds a predictive model for video views and deploys an interactive dashboard for strategic content planning.

> 🎯 Designed for content strategists, media analysts, and creators to forecast video performance and optimize publishing strategies.

---

## 🛠️ Tools & Technologies  

| Category       | Stack                                                                 |
|----------------|----------------------------------------------------------------------|
| Languages      | Python, SQL                                                          |
| Libraries      | Pandas, NumPy, Scikit-learn                                           |
| Platforms      | Jupyter Notebook, VS Code, Streamlit                                 |
| Visualization  | MS Access Dashboard                                                  |
| Techniques     | Data Cleaning, Label Encoding, Regression Modeling, Feature Engineering |

---

## 📦 Dataset Summary  

- **Source:** Aggregated YouTube trending data across multiple countries  
- **Size:** ~100,000 records  
- **Key Columns:**  
  `video_id`, `title`, `channel_title`, `publish_time`, `views`, `likes`, `dislikes`, `comment_count`, `country`, `category_id`, `tags`, `description`  
- **Target Variable:** `views`  
- **Feature Engineering:** Encoded categorical variables, engagement metrics, publish time features  

---

## 📊 Key Insights  

- 👍 **Engagement Drives Views:** Likes and comments are strong predictors of video popularity  
- 🌍 **Country-Specific Trends:** Certain categories trend more consistently in specific regions  
- 📺 **Channel Behavior:** High-performing channels maintain consistent engagement across uploads  
- 🤖 **Model Accuracy:** Regression model predicts view counts with high reliability  
- 🧪 **Interactive Deployment:** Streamlit app enables real-time prediction based on video metadata  

---

## 🗂️ Repository Structure  

| File                          | Purpose                                                       |
|-------------------------------|---------------------------------------------------------------|
| `youtube.sql`                 | SQL queries for data extraction                              |
| `youtube analysis.ipynb`      | Full analysis workflow in Jupyter                            |
| `sqlconnect.py`               | SQL connection script                                         |
| `app.py`                      | Streamlit app for prediction                                 |
| `trending_model.pkl`          | Trained regression model                                     |
| `trending_features.pkl`       | Feature list used in modeling                                |
| `channel_encoder.pkl`         | Label encoder for channel names                              |
| `country_encoder.pkl`         | Label encoder for country names                              |
| `cleaned_youtube.csv`         | Preprocessed dataset                                         |
| `youtube.csv`                 | Raw dataset                                                   |
| `YOUTUBE ANALYSIS DASHBOARD.accdb` | MS Access dashboard for visual insights               |

---

## 📈 Dashboard Preview  

Dashboards are provided via MS Access and include: 
- View distribution by country and category
- Engagement metrics over time
- KPI cards for average views, likes, and comments

<img src="https://image2url.com/images/1755686917071-3ea0c735-c3e5-4289-ae1a-c0ce0c25170f.png" alt="Dashboard Preview" width="600"/>

---

## 🧪 How to Run Locally  

```bash
# Step 1: Clone the repository
git clone https://github.com/aneshraj-data-96/You-Tube-analysis.git

# Step 2: Install dependencies
pip install -r requirements.txt

# Step 3: Launch the Streamlit app
streamlit run app.py
