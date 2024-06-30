# Movies-Analysis-Case-Study!


# Business Task: Enhancing the Success of Movie Franchises

## Task Statement
Identify the factors that contribute to the success of movie franchises and develop strategies to enhance their long-term profitability.

## Explanation
This business task focuses on understanding the key elements that make movie franchises successful over time. By analyzing data related to franchise movies, including box office performance, audience demographics, critical reception, marketing strategies, and franchise longevity, we aim to uncover patterns and insights that can guide decision-making to maximize profitability for both existing and future franchises. The analysis will delve into factors such as franchise popularity, sequel performance, franchise fatigue, franchise universes, and the impact of factors like cast, directors, and genres on franchise success. The ultimate goal is to provide actionable recommendations to movie studios and producers on how to effectively manage and leverage movie franchises for sustained financial success.

## Detailed Business Task Statement

### Objective
The primary objective is to understand the key elements that contribute to the long-term success of movie franchises. By conducting a comprehensive analysis of various data aspects related to franchise movies, the goal is to identify patterns and insights that can inform strategies to maximize profitability and ensure sustained success for both existing and future franchises.

### Scope of Analysis

#### Box Office Performance
- **Total Revenue**: Analyze the box office revenue generated by each franchise and its individual movies.
- **Revenue Trends**: Examine revenue trends across different phases of a franchise, such as initial releases, sequels, and reboots.

#### Audience Demographics
- **Age and Gender**: Investigate the demographics of the audience, including age and gender, to understand who the primary viewers are.
- **Geographic Distribution**: Analyze geographic data to determine regional popularity and performance of franchise movies.

#### Critical Reception
- **Ratings and Reviews**: Assess critical reception through movie ratings and reviews from platforms like IMDb, Rotten Tomatoes, and Metacritic.
- **Award Wins/Nominations**: Consider the impact of awards and nominations on the success and longevity of franchises.

#### Marketing Strategies
- **Promotional Activities**: Evaluate the effectiveness of different marketing strategies, including trailers, social media campaigns, and merchandise.
- **Budget Allocation**: Analyze how marketing budget allocation correlates with box office performance.

#### Franchise Longevity
- **Duration and Frequency**: Examine the lifespan of franchises, including the time between releases and the frequency of new installments.
- **Sustainability**: Assess the sustainability of franchises over time, identifying signs of franchise fatigue and strategies to mitigate it.

#### Franchise Popularity
- **Brand Recognition**: Measure the popularity of franchises based on social media mentions, search trends, and merchandise sales.
- **Fan Engagement**: Look into fan engagement activities, such as conventions, fan clubs, and online communities.

#### Sequel Performance
- **Comparison of Installments**: Compare the performance of sequels to the original movies and identify factors that contribute to successful sequels.
- **Quality Consistency**: Analyze the consistency in quality across sequels in terms of storytelling, production values, and critical reception.

#### Franchise Universes
- **Connected Stories**: Explore the success of franchise universes where multiple movies share interconnected storylines and characters (e.g., Marvel Cinematic Universe).
- **Spin-offs and Prequels**: Investigate the performance and impact of spin-offs and prequels on the overall franchise.

#### Impact of Key Factors
- **Cast and Directors**: Analyze the influence of prominent cast members and directors on the success of franchise movies.
- **Genres**: Examine the impact of different genres and sub-genres on the performance and popularity of franchises.

### Deliverables
1. **Comprehensive Report**: A detailed report covering all aspects of the analysis, including data sources, methodology, key findings, and insights.
2. **Visualizations**: Compelling visualizations to support the analysis, including charts, graphs, and infographics that highlight trends and patterns.
3. **Recommendations**: Actionable recommendations for movie studios and producers to enhance the profitability and longevity of their franchises.
4. **Presentation**: A 30-minute presentation summarizing the analysis, key findings, and recommendations, tailored for stakeholders and decision-makers.

### End Goal
The ultimate goal is to provide movie studios and producers with data-driven insights and strategies to effectively manage and leverage their movie franchises for sustained financial success. By understanding the key factors that contribute to franchise success, studios can make informed decisions on resource allocation, marketing strategies, content development, and audience engagement to maximize their profitability and ensure the long-term viability of their franchises.


# Movie Franchise Analysis

## Data Sources
### Description
We need to select an appropriate dataset that will allow us to analyze movie franchises comprehensively.

### Dataset
We will use the "Movies Dataset" by Rounak Banik, which includes metadata about 45,000 movies, including information on franchises, box office revenue, ratings, genres, release dates, and more.

## Data Cleaning
### Process
Before conducting analysis, we need to clean the dataset to ensure data integrity and reliability.

### Steps
- **Handle missing values:** Identify and address any missing values in the dataset.
- **Remove duplicates:** Check for and eliminate duplicate entries to avoid redundancy.
- **Standardize variable formats:** Ensure consistency in variable formats for easier analysis.
- **Verify data integrity:** Double-check the dataset to ensure accuracy and reliability.

## Analysis
### Summary
Conduct comprehensive analysis to identify factors influencing the success of movie franchises.

### Key Analysis Tasks
- **Identify successful movie franchises:** Determine criteria for defining successful franchises based on box office revenue, audience ratings, and critical acclaim.
- **Analyze franchise performance:** Explore trends in box office revenue, ratings, and audience demographics for franchise movies.
- **Evaluate franchise longevity:** Assess the lifespan and sustainability of movie franchises over time.
- **Identify influential factors:** Analyze the impact of factors such as cast, directors, genres, marketing strategies, and release timing on franchise success.
- **Explore audience preferences:** Investigate audience preferences for specific franchises and genres.
- **Identify successful franchise strategies:** Extract insights from successful franchise models and strategies for long-term profitability.

## Visualizations
### Visual Representation
Create visualizations to present key findings and insights from the analysis.

### Visualization Types
- **Bar charts:** Show comparisons of box office revenue and ratings between different franchises.
- **Line graphs:** Display trends in franchise performance over time.
- **Pie charts:** Illustrate the distribution of genres within successful franchises.
- **Scatter plots:** Explore relationships between variables such as budget and box office revenue.

## Recommendations
### Insights
Based on the analysis, provide actionable recommendations for movie studios and producers.

### Recommendations
- **Invest in strong storytelling:** Emphasize compelling narratives and character development to engage audiences and build franchise loyalty.
- **Maintain consistency:** Ensure continuity in themes, characters, and quality across franchise installments to sustain audience interest.
- **Leverage fan engagement:** Engage with fans through social media, fan events, and merchandise to cultivate a dedicated fan base.
- **Explore expansion opportunities:** Consider spin-offs, prequels, or related content to expand the franchise universe and appeal to broader audiences.
- **Adapt to changing trends:** Stay informed about evolving audience preferences and industry trends to adapt franchise strategies accordingly.

## Presentation
### Delivery
Prepare a presentation to communicate the analysis findings and recommendations effectively.

### Presentation Components
- **Introduction:** Provide an overview of the business task and objectives.
- **Data Analysis:** Present key findings and insights from the analysis, supported by visualizations.
- **Recommendations:** Outline actionable recommendations for maximizing franchise profitability.
- **Conclusion:** Summarize the key takeaways and emphasize the value of data-driven insights for decision-making.

## Action
### Conclusion
Prepare the deliverables for the case study and plan next steps for implementing the recommendations.

### Next Steps
- Compile the presentation slides and supporting materials.
- Review and refine the presentation for clarity and effectiveness.
- Present the findings and recommendations to stakeholders and decision-makers.
- Implement the recommended strategies and monitor their impact on franchise performance.



---

## Loading and Analyzing the Dataset in R

### Step 1: Load and Clean the Data
Let's load the data into R and clean it to ensure it's ready for analysis.

```r
packages <- c("dplyr", "ggplot2", "lubridate", "jsonlite", "tidyr", "purrr")

install_if_needed <- function(package) {
  if (!requireNamespace(package, quietly = TRUE)) {
    install.packages(package)
  }
}

invisible(lapply(packages, install_if_needed))

# Load necessary libraries
lapply(packages, library, character.only = TRUE)

[[1]]
 [1] "knitr"      "kableExtra" "purrr"      "tidyr"      "jsonlite"  
 [6] "lubridate"  "ggplot2"    "dplyr"      "stats"      "graphics"  
[11] "grDevices"  "utils"      "datasets"   "methods"    "base"      

[[2]]
 [1] "knitr"      "kableExtra" "purrr"      "tidyr"      "jsonlite"  
 [6] "lubridate"  "ggplot2"    "dplyr"      "stats"      "graphics"  
[11] "grDevices"  "utils"      "datasets"   "methods"    "base"      

[[3]]
 [1] "knitr"      "kableExtra" "purrr"      "tidyr"      "jsonlite"  
 [6] "lubridate"  "ggplot2"    "dplyr"      "stats"      "graphics"  
[11] "grDevices"  "utils"      "datasets"   "methods"    "base"      

[[4]]
 [1] "knitr"      "kableExtra" "purrr"      "tidyr"      "jsonlite"  
 [6] "lubridate"  "ggplot2"    "dplyr"      "stats"      "graphics"  
[11] "grDevices"  "utils"      "datasets"   "methods"    "base"      

[[5]]
 [1] "knitr"      "kableExtra" "purrr"      "tidyr"      "jsonlite"  
 [6] "lubridate"  "ggplot2"    "dplyr"      "stats"      "graphics"  
[11] "grDevices"  "utils"      "datasets"   "methods"    "base"      

[[6]]
 [1] "knitr"      "kableExtra" "purrr"      "tidyr"      "jsonlite"  
 [6] "lubridate"  "ggplot2"    "dplyr"      "stats"      "graphics"  
[11] "grDevices"  "utils"      "datasets"   "methods"    "base"      


```
# Load the dataset
```r
movies_metadata <- read.csv("movies_metadata.csv", stringsAsFactors = FALSE)
```
# Initial cleaning
```r
movies_clean <- movies_metadata %>%
  filter(!is.na(revenue) & !is.na(budget) & !is.na(release_date) & revenue > 0 & budget > 0) %>%
  mutate(release_date = as.Date(release_date, format = "%Y-%m-%d"))
```
# Create franchise identifiers
```r
movies_clean <- movies_clean %>%
  mutate(franchise = case_when(
    grepl("Star Wars", title, ignore.case = TRUE) ~ "Star Wars",
    grepl("Harry Potter", title, ignore.case = TRUE) ~ "Harry Potter",
    grepl("Avengers", title, ignore.case = TRUE) ~ "Avengers",
    grepl("Batman", title, ignore.case = TRUE) ~ "Batman",
    TRUE ~ "Other"
  ))
if (!requireNamespace("kableExtra", quietly = TRUE)) {
  install.packages("kableExtra")
}
library(kableExtra)
library(knitr)

movies_clean <- data.frame(
  id = c(1, 2, 3, 4, 5, 6),
  title = c("Toy Story", "Jumanji", "Waiting to Exhale", "Heat", "Sudden Death", "GoldenEye"),
  franchise = c("Other", "Other", "Other", "Other", "Other", "Other"),
  budget = c(30000000, 65000000, 16000000, 60000000, 35000000, 58000000),
  revenue = c(373554033, 262797249, 81452156, 187436818, 64350171, 352194034),
  release_date = as.Date(c("1995-10-30", "1995-12-15", "1995-12-22", "1995-12-15", "1995-12-22", "1995-11-16")),
  vote_average = c(7.7, 6.9, 6.1, 7.7, 5.5, 6.6),
  genres_parsed = c("Animation, Comedy, Family", "Adventure, Fantasy, Family", "Comedy, Drama, Romance", "Action, Crime, Drama, Thriller", "Action, Adventure, Thriller", "Adventure, Action, Thriller")
)

movies_clean %>%
  select(id, title, franchise, budget, revenue, release_date, vote_average, genres_parsed) %>%
  head() %>%
  kable() %>%
  kable_styling(bootstrap_options = c("striped", "hover", "condensed"), full_width = F)


```
# Total Revenue Analysis
```r
total_revenue_franchise <- movies_clean %>%
  group_by(franchise) %>%
  summarise(total_revenue = sum(revenue, na.rm = TRUE)) %>%
  arrange(desc(total_revenue))

print(total_revenue_franchise)

A tibble: 1 × 2
  franchise total_revenue
  <chr>             <dbl>
1 Other        1321784461
>

```
# Revenue Trends Analysis
```r
# Examine revenue trends across different phases of a franchise, such as initial releases, sequels, and reboots.
# Total revenue by movie
total_revenue_movie <- movies_clean %>%
  select(title, franchise, revenue) %>%
  arrange(desc(revenue))

# View the top 10 movies by revenue
head(total_revenue_movie, 10)

1                                        Avatar        Other 2787965087
2                  Star Wars: The Force Awakens    Star Wars 2068223624
3                                       Titanic        Other 1845034188
4                                  The Avengers     Avengers 1519557910
5                                Jurassic World        Other 1513528810
6                                     Furious 7        Other 1506249360
7                       Avengers: Age of Ultron     Avengers 1405403694
8  Harry Potter and the Deathly Hallows: Part 2 Harry Potter 1342000000
9                                        Frozen        Other 1274219009
10                         Beauty and the Beast        Other 1262886337



# Revenue trends over time for each franchise
revenue_trends <- movies_clean %>%
  group_by(franchise, release_date) %>%
  summarise(total_revenue = sum(revenue, na.rm = TRUE)) %>%
  arrange(release_date)

# Plot revenue trends over time for each franchise
ggplot(revenue_trends, aes(x = release_date, y = total_revenue, color = franchise)) +
  geom_line() +
  labs(title = "Revenue Trends Over Time by Franchise",
       x = "Release Date",
       y = "Total Revenue") +
  theme_minimal()
```

![Revenue Trends Over Time by Franchise (2)](https://github.com/LOLO-MKHWANAZI/Movies-Analysis-Case-Study/assets/163551783/6de20121-2fb0-4658-8ed0-d7d66a3ba595)

# Analyze Performance Across Different Phases
```r
# Adding a phase identifier
movies_clean <- movies_clean %>%
  mutate(phase = case_when(
    grepl("Episode", title, ignore.case = TRUE) ~ "Sequel",
    grepl("Part", title, ignore.case = TRUE) ~ "Sequel",
    grepl("Reboot", title, ignore.case = TRUE) ~ "Reboot",
    TRUE ~ "Initial Release"
  ))

# Revenue trends by phase
revenue_trends_phase <- movies_clean %>%
  group_by(franchise, phase) %>%
  summarise(total_revenue = sum(revenue, na.rm = TRUE)) %>%
  arrange(desc(total_revenue))

# View revenue trends by phase
print(revenue_trends_phase)
A tibble: 8 × 3
# Groups:   franchise [5]
  franchise    phase           total_revenue
  <chr>        <chr>                   <dbl>
1 Other        Initial Release  459894943588
2 Other        Sequel             6199379106
3 Harry Potter Initial Release    5411061557
4 Star Wars    Initial Release    3967961748
5 Avengers     Initial Release    2973547020
6 Batman       Initial Release    2834906832
7 Star Wars    Sequel             2423715886
8 Harry Potter Sequel             2296305868


# Plot revenue trends by phase
ggplot(revenue_trends_phase, aes(x = phase, y = total_revenue, fill = franchise)) +
  geom_bar(stat = "identity", position = "dodge") +
  labs(title = "Revenue Trends by Phase and Franchise",
       x = "Phase",
       y = "Total Revenue") +
  theme_minimal()
```
# Audience Demographics
```r
# Synthetic dataset for audience demographics
audience_demographics <- data.frame(
  movie_id = c(1, 2, 3, 4, 5),
  age_group = c('18-24', '25-34', '35-44', '45-54', '55+'),
  gender = c('Male', 'Female', 'Male', 'Female', 'Male'),
  viewers_demographics = c(5000, 6000, 3000, 4000, 2000) # renamed column
)

# Synthetic dataset for audience geographic data
audience_geographic <- data.frame(
  movie_id = c(1, 2, 3, 4, 5),
  region = c('North America', 'Europe', 'Asia', 'South America', 'Australia'),
  viewers_geographic = c(10000, 8000, 12000, 5000, 3000) # renamed column
)

# Join audience demographics and geographic data
audience_data <- audience_demographics %>%
  left_join(audience_geographic, by = "movie_id")

# Analyze audience demographics
demographic_summary <- audience_data %>%
  group_by(movie_id, age_group, gender, region) %>%
  summarise(total_viewers_demographics = sum(viewers_demographics, na.rm = TRUE),
            total_viewers_geographic = sum(viewers_geographic, na.rm = TRUE))

# View the demographic summary
print(demographic_summary)
A tibble: 5 × 6
# Groups:   movie_id, age_group, gender [5]
  movie_id age_group gender region        total_viewers_demographics
     <dbl> <chr>     <chr>  <chr>                              <dbl>
1        1 18-24     Male   North America                       5000
2        2 25-34     Female Europe                              6000
3        3 35-44     Male   Asia                                3000
4        4 45-54     Female South America                       4000
5        5 55+       Male   Australia                           2000
# ℹ 1 more variable: total_viewers_geographic <dbl>

# Add a new column for total viewers
demographic_summary <- demographic_summary %>%
  mutate(total_viewers = total_viewers_demographics + total_viewers_geographic)

# Plotting audience demographics
ggplot(demographic_summary, aes(x = age_group, y = total_viewers, fill = gender)) +
  geom_bar(stat = "identity", position = "dodge") +
  facet_wrap(~ region) +
  labs(title = "Audience Demographics by Age Group, Gender, and Region",
       x = "Age Group",
       y = "Total Viewers") +
  theme_minimal()

# Print the structure of audience_data
str(audience_data)
data.frame':	5 obs. of  6 variables:
 $ movie_id            : num  1 2 3 4 5
 $ age_group           : chr  "18-24" "25-34" "35-44" "45-54" ...
 $ gender              : chr  "Male" "Female" "Male" "Female" ...
 $ viewers_demographics: num  5000 6000 3000 4000 2000
 $ region              : chr  "North America" "Europe" "Asia" "South America" ...
 $ viewers_geographic  : num  10000 8000 12000 5000 3000

```
# Geographic Distribution

## Geographic Distribution
Geographic data can show regional popularity. We'll need a dataset that includes geographic information.

### Analyze Geographic Distribution
```R
geo_summary <- audience_data %>%
  group_by(region) %>%
  summarise(total_viewers = sum(viewers_geographic, na.rm = TRUE))

print(geo_summary)
A tibble: 5 × 2
  region        total_viewers
  <chr>                 <dbl>
1 Asia                  12000
2 Australia              3000
3 Europe                 8000
4 North America         10000
5 South America          5000
```
# Plotting Geographic Distribution
```R
ggplot(geo_summary, aes(x = region, y = total_viewers, fill = region)) +
  geom_bar(stat = "identity", position = "dodge") +
  labs(title = "Total Viewers by Region",
       x = "Region",
       y = "Total Viewers") +
  theme_minimal()
```
# Critical Reception
**We'll analyze movie ratings and reviews. This might involve scraping or loading data from platforms like IMDb, Rotten Tomatoes, and Metacritic.**
```R
# Synthetic Dataset for Movie Ratings
movie_ratings <- data.frame(
  movie_id = c(1, 2, 3, 4, 5),
  rating = c(7.5, 8.0, 6.5, 7.0, 5.5),
  reviews = c(1500, 2000, 800, 1200, 600)
)

movies_with_ratings <- merge(movies_clean, movie_ratings, by.x = "id", by.y = "movie_id")

ratings_summary <- movies_with_ratings %>%
  group_by(franchise) %>%
  summarise(avg_rating = mean(rating, na.rm = TRUE),
            num_reviews = sum(reviews, na.rm = TRUE))

print(ratings_summary)
A tibble: 1 × 3
  franchise avg_rating num_reviews
  <chr>          <dbl>       <dbl>
1 Other            5.5         600
```
# Plotting Critical Reception
```R
ggplot(ratings_summary, aes(x = franchise, y = avg_rating, fill = franchise)) +
  geom_bar(stat = "identity") +
  labs(title = "Average Rating by Franchise",
       x = "Franchise",
       y = "Average Rating") +
  theme_minimal()
```
# Marketing Strategies
**We will need data on marketing budgets and promotional activities.**
```R
# Synthetic Dataset for Marketing Spend
marketing_spend <- data.frame(
  movie_id = c(1, 2, 3, 4, 5),
  marketing_budget = c(2000000, 3000000, 1500000, 2500000, 1000000),
  revenue = c(50000000, 60000000, 30000000, 45000000, 25000000)
)

marketing_spend <- marketing_spend %>%
  rename(marketing_revenue = revenue)

movies_with_marketing <- merge(movies_clean, marketing_spend, by.x = "id", by.y = "movie_id")

marketing_summary <- movies_with_marketing %>%
  group_by(franchise) %>%
  summarise(total_marketing_spend = sum(marketing_budget, na.rm = TRUE),
            total_revenue = sum(marketing_revenue, na.rm = TRUE))

print(marketing_summary)

A tibble: 1 × 3
  franchise total_marketing_spend total_revenue
  <chr>                     <dbl>         <dbl>
1 Other                   1000000      25000000
```
# Plotting Marketing Spend vs Revenue
```R
ggplot(marketing_summary, aes(x = total_marketing_spend, y = total_revenue, color = franchise)) +
  geom_point() +
  labs(title = "Marketing Spend vs Revenue by Franchise",
       x = "Total Marketing Spend",
       y = "Total Revenue") +
  theme_minimal()
```
# Franchise Longevity
**We'll examine the lifespan of franchises, including the time between releases and the frequency of new installments.**
```R
# Calculate the Duration and Frequency of Franchise Movies
franchise_lifespan <- movies_clean %>%
  group_by(franchise) %>%
  summarise(start_year = min(year(release_date)),
            end_year = max(year(release_date)),
            num_movies = n()) %>%
  mutate(duration = end_year - start_year)

print(franchise_lifespan)

A tibble: 5 × 5
  franchise    start_year end_year num_movies duration
  <chr>             <dbl>    <dbl>      <int>    <dbl>
1 Avengers           1998     2015          3       17
2 Batman             1989     2017          9       28
3 Harry Potter       2001     2011          8       10
4 Other              1915     2017       5354      102
5 Star Wars          1977     2016          7       39
```
# Plotting Franchise Longevity
```R
ggplot(franchise_lifespan, aes(x = franchise, y = duration, fill = franchise)) +
  geom_bar(stat = "identity") +
  labs(title = "Franchise Longevity",
       x = "Franchise",
       y = "Duration (Years)") +
  theme_minimal()
```

# Franchise Popularity
**Popularity can be measured by social media mentions, search trends, and merchandise sales.**
```R
# Synthetic Dataset for Franchise Popularity
franchise_popularity <- data.frame(
  movie_id = c(1, 2, 3, 4, 5),
  social_media_mentions = c(50000, 80000, 45000, 60000, 30000),
  merchandise_sales = c(1000000, 1500000, 800000, 1200000, 600000)
)

movies_with_popularity <- merge(movies_clean, franchise_popularity, by.x = "id", by.y = "movie_id")

popularity_summary <- movies_with_popularity %>%
  group_by(franchise) %>%
  summarise(social_media_mentions = sum(social_media_mentions, na.rm = TRUE),
            merchandise_sales = sum(merchandise_sales, na.rm = TRUE))

print(popularity_summary)

A tibble: 1 × 3
  franchise social_media_mentions merchandise_sales
  <chr>                     <dbl>             <dbl>
1 Other                     30000            600000
```
# Plotting Franchise Popularity
```R
ggplot(popularity_summary, aes(x = social_media_mentions, y = merchandise_sales, color = franchise)) +
  geom_point() +
  labs(title = "Franchise Popularity",
       x = "Social Media Mentions",
       y = "Merchandise Sales") +
  theme_minimal()
```
# Sequel Performance
**Compare the performance of sequels to the original movies and identify factors that contribute to successful sequels.**
```R
# Identify Sequels Based on Title Keywords
movies_with_sequels <- movies_clean %>%
  mutate(sequel = ifelse(grepl("Part|Episode|II|III|IV|V", title, ignore.case = TRUE), "Sequel", "Original"))

sequel_performance <- movies_with_sequels %>%
  group_by(franchise, sequel) %>%
  summarise(avg_revenue = mean(revenue, na.rm = TRUE))

print(sequel_performance)

A tibble: 9 × 3
# Groups:   franchise [5]
  franchise    sequel   avg_revenue
  <chr>        <chr>          <dbl>
1 Avengers     Sequel    991182340 
2 Batman       Original  218861185 
3 Batman       Sequel    507246574 
4 Harry Potter Original  901843593.
5 Harry Potter Sequel   1148152934 
6 Other        Original   86920851.
7 Other        Sequel     87825480.
8 Star Wars    Original  991990437 
9 Star Wars    Sequel    807905295.
```
# Plotting Sequel Performance
```R
ggplot(sequel_performance, aes(x = sequel, y = avg_revenue, fill = franchise)) +
  geom_bar(stat = "identity", position = "dodge") +
  labs(title = "Sequel Performance vs Original",
       x = "Movie Type",
       y = "Average Revenue") +
  theme_minimal()
```
# Franchise Universes
**Explore the success of franchise universes where multiple movies share interconnected storylines and characters.**
```R
# Synthetic Dataset for Connected Movies
connected_movies <- data.frame(
  movie_id = c(1, 2, 3, 4, 5),
  connected_universe = c('Marvel', 'DC', 'Star Wars', 'Harry Potter', 'Transformers')
)

movies_with_connected <- merge(movies_clean, connected_movies, by.x = "id", by.y = "movie_id")

connected_summary <- movies_with_connected %>%
  group_by(franchise, connected_universe) %>%
  summarise(total_revenue = sum(revenue, na.rm = TRUE))

print(connected_summary)

A tibble: 1 × 3
# Groups:   franchise [1]
  franchise connected_universe total_revenue
  <chr>     <chr>                      <dbl>
1 Other     Transformers             4300000
```
# Plotting Connected Universe Performance
```R
ggplot(connected_summary, aes(x = connected_universe, y = total_revenue, fill = franchise)) +
  geom_bar(stat = "identity", position = "dodge") +
  labs(title = "Performance of Connected Universes",
       x = "Connected Universe",
       y = "Total Revenue") +
  theme_minimal()
```
#Impact of Key Factors
**Analyze the influence of prominent cast members and directors on the success of franchise movies, as well as the impact of different genres.**
```R
# Synthetic Dataset for Key Factors
key_factors <- data.frame(
  movie_id = c(1, 2, 3, 4, 5),
  key_factor = c('Director', 'Lead Actor', 'Genre', 'Marketing', 'Budget')
)

movies_with_factors <- merge(movies_clean, key_factors, by.x = "id", by.y = "movie_id")

factor_summary <- movies_with_factors %>%
  group_by(franchise, key_factor) %>%
  summarise(avg_revenue = mean(revenue, na.rm = TRUE))

print(factor_summary)
A tibble: 1 × 3
# Groups:   franchise [1]
  franchise key_factor avg_revenue
  <chr>     <chr>            <dbl>
1 Other     Budget         4300000
```
# Plotting the Impact of Key Factors
```R
ggplot(factor_summary, aes(x = key_factor, y = avg_revenue, fill = franchise)) +
  geom_bar(stat = "identity", position = "dodge") +
  labs(title = "Impact of Key Factors on Franchise Revenue",
       x = "Key Factor",
       y = "Average Revenue") +
  theme_minimal()
```
# Example Movies_clean with Parsed Genres
```R
movies_clean <- data.frame(
  id = c(1, 2, 3),
  title = c("Movie 1", "Movie 2", "Movie 3"),
  genres = c('[{"id": 16, "name": "Animation"}, {"id": 18, "name": "Drama"}]',
             '[{"id": 12, "name": "Adventure"}, {"id": 14, "name": "Fantasy"}]',
             '[{"id": 28, "name": "Action"}, {"id": 12, "name": "Adventure"}]'),
  genres_parsed = c("Animation, Drama", "Adventure, Fantasy", "Action, Adventure")
)

genre_summary <- movies_clean %>%
  separate_rows(genres_parsed, sep = ", ") %>%
  group_by(genres_parsed) %>%
  summarise(count = n())
```
# Plotting Genre Summary
```R
library(ggplot2)

ggplot(genre_summary, aes(x = genres_parsed, y = count, fill = genres_parsed)) +
  geom_bar(stat = "identity") +
  labs(title = "Genre Distribution",
       x = "Genres",
       y = "Count") +
  theme_minimal() +
  theme(axis.text.x = element_text(angle = 45, hjust = 1))



# Conclusion
```r
# Summarize findings
summary_findings <- list(
  "Top Franchises" = total_revenue_franchise,
  "Revenue Trends" = revenue_trends,
  "Revenue by Phase" = revenue_trends_phase,
  "Audience Demographics" = demographic_summary
)

# Print summary findings
print(summary_findings)

$`Top Franchises`
# A tibble: 1 × 2
  franchise total_revenue
  <chr>             <dbl>
1 Other        1321784461

$`Revenue Trends`
# A tibble: 4 × 3
# Groups:   franchise [1]
  franchise release_date total_revenue
  <chr>     <date>               <dbl>
1 Other     1995-10-30       373554033
2 Other     1995-11-16       352194034
3 Other     1995-12-15       450234067
4 Other     1995-12-22       145802327

$`Revenue by Phase`
# A tibble: 1 × 3
# Groups:   franchise [1]
  franchise phase           total_revenue
  <chr>     <chr>                   <dbl>
1 Other     Initial Release    1321784461

$`Audience Demographics`
# A tibble: 5 × 7
# Groups:   movie_id, age_group, gender [5]
  movie_id age_group gender region        total_viewers_demographics
     <dbl> <chr>     <chr>  <chr>                              <dbl>
1        1 18-24     Male   North America                       5000
2        2 25-34     Female Europe                              6000
3        3 35-44     Male   Asia                                3000
4        4 45-54     Female South America                       4000
5        5 55+       Male   Australia                           2000
# ℹ 2 more variables: total_viewers_geographic <dbl>,
#   total_viewers <dbl>

>
```
# Summary of Findings

## 1. Top Franchises
The dataset revealed only one franchise category labeled as "Other," which generated a total revenue of approximately $1,321,784,461.

## 2. Revenue Trends
The revenue trends over time for the "Other" franchise showed the following:
- On 1995-10-30, the revenue was approximately $373,554,033.
- On 1995-11-16, the revenue was approximately $352,194,034.
- On 1995-12-15, the revenue was approximately $450,234,067.
- On 1995-12-22, the revenue was approximately $145,802,327.

## 3. Revenue by Phase
The analysis by phase revealed that the total revenue for the "Other" franchise during the initial release phase was approximately $1,321,784,461.

## 4. Audience Demographics
The audience demographics data provided insights into viewers by age group, gender, and region:
- **18-24, Male, North America:** 5,000 viewers
- **25-34, Female, Europe:** 6,000 viewers
- **35-44, Male, Asia:** 3,000 viewers
- **45-54, Female, South America:** 4,000 viewers
- **55+, Male, Australia:** 2,000 viewers

The dataset also included geographic data for these viewers:
- **North America:** 10,000 viewers
- **Europe:** 8,000 viewers
- **Asia:** 12,000 viewers
- **South America:** 5,000 viewers
- **Australia:** 3,000 viewers

Combining the demographic and geographic data, the total viewers were calculated for each group.
