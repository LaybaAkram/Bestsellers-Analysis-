# Bestsellers-Analysis
A simple pandas script that analyzes a dataset of Amazon bestselling books, looking at top authors and average ratings by genre.

## What it does
`analysis.py` reads `bestsellers.csv` and:
1. Removes duplicate rows.
2. Renames columns for clarity (`Name` → `Title`, `Year` → `Publication Year`, `User Rating` → `Rating`).
3. Ensures the `Price` column is numeric.
4. Counts how many times each author appears in the bestseller list, and saves the top 10 authors to `top_author.csv`.
5. Calculates the average rating per genre, and saves the results to `avg_rating_by_genre.csv`.

## Requirements
```bash
pip install pandas
```

## Usage
```bash
python analysis.py
```
This will print the author counts and average ratings by genre to the console, and regenerate `top_author.csv` and `avg_rating_by_genre.csv`.

## Files
- `analysis.py` — the analysis script
- `bestsellers.csv` — source dataset of bestselling books (columns: Title, Author, Rating, Reviews, Price, Publication Year, Genre)
- `top_author.csv` — output: top 10 most frequent authors
- `avg_rating_by_genre.csv` — output: average rating by genre
