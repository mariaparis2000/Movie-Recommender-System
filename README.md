# 🎬 CinemaMatch: Content-Based Movie Recommender

## 📌 Project Overview
As part of my Master’s in Business Analytics, I developed this movie recommendation engine. The goal is to solve the "choice paralysis" in streaming platforms by suggesting movies based on the user's personal tastes, focusing on director, genre, and lead actors.

## 🛠️ Data & Methodology
The project uses a dataset of the **Top 1000 IMDB Movies**. The core logic follows a **Natural Language Processing (NLP)** approach:

1.  **Data Cleaning:** Handled missing values and converted financial data (`Gross` revenue) from strings to numeric formats for potential analysis.
2.  **Feature Engineering:** Created a "Metadata Soup" (a single string containing the genre, director, and main stars) to build a unique profile for each movie.
3.  **Vectorization:** Used `CountVectorizer` to transform text data into a mathematical matrix.
4.  **Similarity Metric:** Applied **Cosine Similarity** to calculate the distance between movie vectors.

## 💻 Tech Stack
* **Language:** Python 3.13
* **Environment:** VS Code / Jupyter Notebooks
* **Libraries:** Pandas, Scikit-Learn (ML), NumPy

## 🚀 How to Run

Pre-requisites: [Pandas](https://pandas.pydata.org/), Python 3.13

```bash
pip install -r requirements.txt ```

To get recommendations, simply run the function in your notebook or use the following command structure:

python main.py --title "Inception"
