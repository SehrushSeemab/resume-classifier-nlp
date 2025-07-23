# Resume Classifier & Job Market Insights (NLP Project)

A Natural Language Processing (NLP) project that classifies resumes into job categories using machine learning and extracts key insights from resume text. This project is designed to help recruiters and HR professionals automatically categorize and analyze resume data for better decision-making.

## 🚀 Project Overview

- 📂 **Input**: Resume texts and their corresponding job categories
- 🧠 **Tech**: NLP preprocessing, TF-IDF, and classification models (Logistic Regression, SVM, etc.)
- 📊 **Output**: Resume classification + data visualizations for job market trends

---

## 📌 Goals

- Build a machine learning pipeline to classify resumes into categories
- Apply NLP techniques to clean and process real-world textual data
- Visualize common skills and trends across different job roles
- Make the project publicly available to contribute to an open-source portfolio

---

## 🛠️ Methodology

1. **Data Collection**  
   Used publicly available resume dataset from [Kaggle](https://www.kaggle.com/datasets/andrewmvd/resume-dataset)

2. **Data Cleaning & Preprocessing**  
   - Lowercasing, punctuation removal  
   - Stopwords removal  
   - Text normalization with NLTK

3. **Feature Extraction**  
   - TF-IDF vectorization of cleaned text

4. ### 🧪 Models Used

- **TF-IDF Vectorizer**
- **Random Forest Classifier**
- Accuracy: ~78.8% on test data
- Classification report shows strong performance on job roles like DevOps, Mechanical Engineer, Java Developer, and more

5. ### 🛠️ Tools & Technologies

- Python
- Pandas, NumPy
- scikit-learn
- NLTK
- Jupyter Notebook
- Matplotlib / Seaborn (for visualization)


6. ### 📂 Project Structure

resume-job-classifier/
├── data/ # Processed dataset
├── notebooks/ # Jupyter notebooks
│ ├── 01_EDA_data_cleaning.ipynb
│ ├── 02_model_training_evaluation.ipynb
│ └── 03_model_training_and_visualization_improved.ipynb
├── scripts/
│ └── predict_resume.py # Script to predict job role from input resume
├── README.md
├── requirements.txt

7. ### 🧪 Model Evaluation Summary
---Metric   	  |    ---Baseline Model (02)|  	---Improved Model (03)
Accuracy         |   	78.8%                  	|82.0%
Weighted
F1-Score         	78%	                        |81%
Avg. Precision   |	79%                  	   |82%
Avg. Recall      	|77%	                        |80%

Key Improvements:

Applied better preprocessing and text cleaning.

Switched from baseline logistic regression to a tuned classifier.

Improved class balance and support visualization.

Visual Insights:

Confusion matrices clearly show better separation across classes.

Precision/Recall heatmaps reflect gains in specific domains like Business Analyst, Aviation, Digital Media, etc.

Classes like Blockchain and React Developer remain low-support but are now handled more robustly.


### 🚀 How to Use

1. Clone the repository:
```bash
git clone https://github.com/SehrushSeemab/resume-job-classifier.git
cd resume-job-classifier
Install dependencies:

pip install -r requirements.txt
Run the prediction script:

python scripts/predict_resume.py "Paste your resume text here"
✨ Output Example

Predicted Category: Data Science
🤝 Contributions
Contributions, ideas, and improvements are welcome!

