# Module 1 Final Project

Amin Nazerzadeh & Kevin Evans

## Introduction

With many industries currently crippled by the coronavirus pandemic, embarking on a new endeavor can be a very risky decision. At the same time, though, it is also a time of great opportunity. While the production of live-action cinema is currently impossible, the world of animation has been gaining respect in recent times, and could be a lucrative business to venture into. To support this theory, we have collected, sorted, and analyzed information from the Movie Database in order to answer these questions:

<ol>
<li>What is the trend of animated movies over previous 10 years?
<li>Who are the current competitors in this space?
<li>What are the top-earning animated movies?
<li>What is the correlation between the costs of making animated movies and their earnings, and how does this compare to non-animated movies?
</ol>

## Libraries used

To assist us in our research, we utilized the following libraries:

<ul>
<li>Pandas - data cleaning and analysis
<li>Matplotlib - data visualization
<li>Seaborn - data visualization
<li>Requests - api calls and webscrapping
<li>BeauitfulSoup - webscrapping
<li>Re - regular expression searches
</ul>

## Part 1: Data Collection

For our data, we made use of the services provided by The Movie Database (TMDb). We used a large collection of movies from TMDb provided by the Flatiron School, and as well, in order to supplement that data for our specific interest (animated films) we connected to TMDb’s API, collecting titles and details for an addition 10,000 animated films.

In an effort to further augment our data, we built a web scraper to find a movie’s budget on the Internet Movie Database (IMDb) allowing us to fill in potentially missing values. However, from comparing samples of scrapped data against the data collected from our API requests, we found that this method only had the potential to add 1% more data, and thus we decided to not implement the web scraper, saving it for potential future development.

## Part 2: Data Cleaning

While our data set was robust, many of the values were lacking the information we needed. In order to make our analysis viable, we segmented data by genre (animation vs non animation), made data frames including only actionable data, and converted several columns from strings to numeric data.

## Part 3: Analysis

After formatting our data into a useable state, we used various categorization and statistical analysis methods to find answers to our business questions.

<ol>
<li>What is the trend of animated movies over previous 10 years?</li>

As is clearly shown in our chart <em>Number of Animated movies produced over the previous 10 years</em> the production of animated movies has jumped up in the past decade, going from less than 200 in 2010 to a peak near 1000 in 2017. While it has slightly lowered to near 900 in 2019, the industry is clearly stronger now than it was in the past.

<li>
Who are the current competitors in this space?</li>

From our chart <em>Animation Movies made by Different Companies Over the 10 Years Period</em> you can that Disney (labeled as “BV” for “Buena Vista” one of their subsidiaries) leads the market with over 30 animated releases in the last 10 years. While the top 5 companies are relatively prolific, the bottom 5 have put out on average less than one animated film per year, meaning that this is a feasible market to become a leader in.

<li>What are the top-earning animated movies?</li>

From the chart <em>Top Earning Animated Movies</em> we can see a rather homogenous group of movies. From top earner to 10th there is only a 25% difference in revenue, and of these 10 movies 8 are from Disney, with the remaining two (of the Despicable Me franchise) being made by Universal.

<li>What is the correlation between the costs of making animated movies and their earnings, and how does this compare to non-animated movies?</li>

From our charts <em>Non-animated Movies, Budget vs Gross (in millions)</em> and <em>Animated Movies, Budget vs Gross (in millions)</em> We can see the relationships in budgets versus revenues for animated and non-animated movies. As well, from calculating the correlation of these two factors we can see that there is a slightly higher correlation between budget and revenue for non-animated films (0.80) than for animated films (0.71). While this data point means that you may make more, or less than a non-animated film for a given budget, by comparing it with the ratio of average budget to average revenue we can see that on average animated film make more (3.55 times budget) than non-animated films (3.05 times budget).
