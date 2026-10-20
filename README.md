# Resume / Candidate Screening System

## Overview
A Python-based resume screening prototype that compares candidate resumes against a job description, ranks candidates, extracts predefined skills, and highlights matched and missing skills.

## Features
- Resume text preprocessing
- TF-IDF vectorization and cosine similarity
- Keyword-based skill extraction
- Candidate ranking using a combined score
- Matched and missing skills reports
- Candidate ranking visualization

## Technologies
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Jupyter Notebook

## Dataset
The project uses the Resume Dataset available on Kaggle:
https://www.kaggle.com/datasets/snehaanbhawal/resume-dataset

Download the dataset separately and update the notebook's dataset path before running it.

## How to Run
1. Clone or download this repository.
2. Install the dependencies:
   `pip install -r requirements.txt`
3. Download the dataset and configure its path.
4. Open `Resume_Candidate_Screening.ipynb` in Jupyter Notebook or VS Code.
5. Run the notebook cells in order.

## Scoring
The prototype combines text similarity and detected skill match:

`Final Score = 0.60 × Text Similarity + 0.40 × Skill Match`

This is a demonstration heuristic, not a validated hiring prediction.

## Limitations
- Skill extraction uses predefined keywords and aliases.
- Missing skills indicate that a keyword was not detected, not necessarily that the candidate lacks that skill.
- Ranking results should be reviewed by a human and should not be used as the sole basis for hiring decisions.

## Future Improvements
- Expand skill coverage and synonym detection.
- Build a Streamlit interface.
- Evaluate ranking quality against manually reviewed examples.
- Add privacy and fairness testing.
