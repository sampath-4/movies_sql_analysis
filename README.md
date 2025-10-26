🎬 Movies Database Analysis
Overview

This project analyzes a movie ratings dataset to extract meaningful insights about movies, users, and ratings. It demonstrates advanced SQL skills, including joins, aggregations, window functions, and date functions, as well as the ability to derive actionable business insights from raw data.

📂 Database Structure

The project uses a relational database with three tables:

movies
| Column | Type | Description |
|----------|------------|-------------------------|
| movieId | INT (PK) | Unique movie identifier |
| title | VARCHAR | Movie title |
| genres | VARCHAR | Genres (comma-separated)|

users
| Column | Type | Description |
|-----------|------------|-----------------------------|
| userId | INT (PK) | Unique user identifier |
| age | INT | Age of the user |
| gender | CHAR(1) | Gender (M/F) |
| occupation| VARCHAR | User occupation |
| zip_code | VARCHAR | Zip code |

ratings
| Column | Type | Description |
|-----------|------------|-----------------------------|
| userId | INT (FK) | Reference to users table |
| movieId | INT (FK) | Reference to movies table |
| rating | INT | User rating (1–5) |
| timestamp | BIGINT | Unix timestamp of rating |

🔹 Key SQL Skills Demonstrated

Joins: INNER JOIN across multiple tables

Aggregations: AVG, COUNT, SUM

GROUP BY & HAVING for grouped analysis

Window Functions: RANK() OVER (PARTITION BY …)

CASE Statements: Age group analysis

Date Functions: strftime() to analyze monthly trends

🔹 Business Questions Answered

Top 10 movies by average rating

Top 10 movies by number of ratings

Average rating by genre

Top users by average rating given

Average rating by gender and age group

Top-rated movie in each genre

Rare movies with high ratings but few reviews

Users with most ratings

Ratings trends over months

📊 Insights

Genres X, Y, Z consistently have higher average ratings.

Users aged 26–35 tend to rate movies highest on average.

Top-rated movies often belong to [list top genres].

The most active users are highly engaged in rating movies, highlighting core audience segments.

Monthly trends indicate peak rating activity during holidays and major movie release periods.

🔹 Tools Used

SQL (MySQL / PostgreSQL / SQLite)

Optional: Python (Pandas/Matplotlib) or Power BI for visualizations

💼 How to Run

Clone the repository:

git clone <your-repo-url>


Import the movies_db schema into your SQL server.

Run the provided SQL queries in the SQL console to replicate analysis.

Optionally, connect to Python/Power BI to visualize insights.

🔹 Future Enhancements

Build an AI-powered insights generator to automatically summarize trends.

Add recommendation system queries to suggest movies for users.

Integrate visual dashboards with Power BI or Tableau.
