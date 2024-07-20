# movieMetrics
This project is performing an analysis on movie budget and profit data from a DataFrame called `imdb_budgets_df` to make recommendations about movie production budgets and genres. Here’s a breakdown of the steps and goals of the project:

## Question 1: What are the most profitable movies and how much should you spend?

1. **Calculate Profit and Profit Margin**:
    - **Profit**: Calculated as `Worldwide Gross - Production Budget`.
    - **Profit Margin**: Usually calculated as `Profit / Production Budget`.

2. **Adjust for Inflation**:
    - Create `Adjusted_Budget` and `Adjusted_Profit` columns accounting for an average inflation rate of 6.8%.

3. **Identify Profitable Movies**:
    - Filter movies with `Profit > 0` into a new DataFrame `profitable_movies_df`.

4. **Sort and Rank Movies by Adjusted Profit**:
    - Rank movies based on `Adjusted_Profit` to identify the most successful ones.

5. **Scatter Plot Analysis**:
    - Plot a scatter plot to understand the relationship between budget and profit.

6. **Analyze Top 25 Movies**:
    - Identify the most successful 25 movies in terms of profit and profit margin.
    - Determine the median budget and profit margin for these movies.

7. **Set Budget Recommendations**:
    - Based on the analysis, recommend a budget for producing a movie.
    - Initially found a median budget of $1,152,000,000 and profit margin of 85% for the top 25 movies.
    - For all profitable movies, found a median budget of $316,320,000 and profit margin of 62%.

8. **Filter Data for Higher Profit Margins**:
    - Filter movies with a profit margin of 75% or greater and a budget greater than $316,320,000.
    - After filtering, still have 393 movies.
    - Median budget is $677,600,000 with a median profit margin of 84%.

9. **Final Budget Recommendation**:
    - Recommend budgeting approximately $678,000,000 to achieve a profit margin above 80%.

## Question 2: Which movie genres are most commonly produced and does quantity equate to higher net profits?

1. **Analyze Genre Production**:
    - Identify the most commonly produced genres.

2. **Profitability of Genres**:
    - Group movies by genre and calculate the average net profit for each genre.
    - Identify genres with the highest median net profit (e.g., Animation, Adventure, Sci-Fi).

3. **Profit Margins by Genre**:
    - Determine genres with the most desirable profit margins.
    - Note any anomalies or outliers (e.g., Film Noir has a high profit margin but with a small sample size).

4. **Percentage of Total Net Profit by Genre**:
    - Determine the percentage of total net profit that each genre accounts for.
    - Identify which genres contribute most to overall profits.

## Conclusions and Recommendations

1. **Budget Recommendations**:
    - For profitable movie production, a budget of around $678,000,000 is recommended to achieve a profit margin above 80%.

2. **Genre Focus**:
    - Focus on the top 6 most profitable movie genres: Adventure, Action, Comedy, Drama, Sci-Fi, and Animation.
    - Additional focus on Sci-Fi and Animation due to less competition and higher potential profits.

## Key Insights

- **High Budget and High Profit Margin**: The most profitable movies tend to have high budgets but also achieve high profit margins.
- **Profit Margins and Budget Relationship**: While a higher budget often correlates with higher profits, there's a caution against overspending as it can negatively affect profit margins.
- **Genre Profitability**: Less commonly produced genres like Sci-Fi and Animation can be highly profitable, offering opportunities in less saturated markets.

### Summary

The project aims to guide movie production decisions by analyzing historical data on movie budgets, profits, and genres. By identifying the most profitable movies and genres, the project recommends optimal budget allocations and strategic focus areas to maximize profitability in future productions.
