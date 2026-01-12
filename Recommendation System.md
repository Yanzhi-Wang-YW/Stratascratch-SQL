```md
# Recommendation System

Last Updated: January 2026

Medium The difficulty is Medium, because the solution involves complex logic that requires joining multiple datasets and applying conditions to compare and filter results. This multi-step process entails identifying relationships between various entities and ensuring that users are recommended pages that none of their friends follow, adding layers of complexity to the task.

ID 2081

204

You are given the list of Facebook friends and the list of Facebook pages that users follow. Your task is to create a new recommendation system for Facebook. For each Facebook user, find pages that this user doesn't follow but at least one of their friends does. Output the user ID and the ID of the page that should be recommended to this user.

### Tables

users\_friends

users\_pages

### More about this question

### Companies

Meta

### Job Positions

Data Engineer

Data Scientist

BI Analyst

Data Analyst

ML Engineer

### Topic Family

Column Manipulation

Data Cleaning

DataFrame Operations

Data Manipulation &amp; Wrangling

Data Retrieval Basics

Filtering Data

Joins Merging

Joins &amp; Merging

Joins &amp; Set Operations

Join Types

Merge Operations

Null Handling

Tidyverse Essentials

### Topic Functions

anti\_join()

distinct()

drop\_duplicates()

inner\_join()

isna()

merge()

select()

* * *

Hints Expected Output

* * *

### users\_friends

Preview

| user\_id | friend\_id |
|----------|------------|
| 1        | 2          |
| 1        | 4          |
| 1        | 5          |
| 2        | 1          |
| 2        | 3          |
| 2        | 4          |
| 2        | 5          |
| 3        | 2          |
| 4        | 1          |
| 4        | 2          |
| 5        | 1          |
| 5        | 2          |

friend\_id:bigintuser\_id:bigint

### users\_pages

Preview

| user\_id | page\_id |
|----------|----------|
| 1        | 21       |
| 1        | 25       |
| 2        | 25       |
| 2        | 23       |
| 2        | 24       |
| 2        | 28       |
| 2        | 21       |
| 3        | 25       |
| 3        | 24       |
| 5        | 23       |
| 5        | 28       |
```

```sql
WITH users_friend_follow AS (
    SELECT DISTINCT users_friends.user_id, users_pages.page_id 
    FROM users_friends 
    INNER JOIN users_pages 
    ON users_friends.friend_id = users_pages.user_id  
), 
recommended_page AS (
    SELECT DISTINCT users_friend_follow.*   
    FROM users_friend_follow 
    LEFT JOIN users_pages 
    ON users_friend_follow.user_id = users_pages.user_id 
    AND users_friend_follow.page_id = users_pages.page_id 
    WHERE users_pages.page_id IS NULL 
) 
SELECT * 
FROM recommended_page 
ORDER BY user_id ASC, page_id ASC
```
