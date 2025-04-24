Movie Rating Prediction 

👤 Author
Manan Agarwal
B.Tech CCE, Manipal University Jaipur  
[GitHub](https://github.com/Manan-Agarwal-1) • [LinkedIn](https://www.linkedin.com/in/manan-agarwal-9b561135b?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

Task Objectives

The goal of this project is to develop a machine learning model that predicts the IMDb rating of a movie based on key features such as:

- Duration
- Number of Votes
- Genre(s)
- Director

We also engineer informative features like:
Director Success Rate** – average rating of movies by the same director
Genre Average Rating** – average rating of movies in the same genre(s)


 How to Run This Project


1. Install Requirements

```bash
pip install -r requirements.txt
```

2. Run the Code

```bash
python movie.py
```

The script will:
- Train a predictive model (if not already saved)
- Prompt the user to input details of a new movie
- Output the predicted IMDb rating


Features Used

| Feature             | Description                                               |
|--------------------|-----------------------------------------------------------|
| `Duration`         | Runtime of the movie in minutes                           |
| `Votes`            | Number of IMDb votes received                             |
| `Director_Success` | Average IMDb rating of other movies by the same director  |
| `Genre_Avg_Rating` | Average IMDb rating of movies with similar genre          |
| `Genre`            | One-hot encoded genres (Drama, Comedy, etc.)              |


Evaluation Criteria

| Metric         | Description                                         |
|----------------|-----------------------------------------------------|
| RMSE           | Root Mean Square Error for model performance        |
| Model          | `RandomForestRegressor` from scikit-learn           |
| Data Handling  | Missing values, outliers, and category encoding     |
| Code Quality   | Clean, modular, and well-commented code             |


Project Structure

```
movie-rating-prediction/
│
├── IMDb Movies India.csv      # Dataset
├── movie.py                   # Main prediction script
├── model.pkl                  # Saved ML model (auto-generated)
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation
```



Sample Output

```bash
--- Enter New Movie Details ---
Enter duration (in minutes): 105
Enter number of votes: 2300
Enter director name: Zoya Akhtar
Enter genre(s) (comma separated): Drama, Musical

🎬 Predicted Movie Rating: 7.88
