When browsing the [dataisbeautiful subreddit](https://www.reddit.com/r/dataisbeautiful/), I came across a visualization for storm damages by season. At the time, it was during hurricane season so storms were being talked in the news a lot, so I knew something was up with the data. The poster had reported spring as the season where most damages occurred, but summer and fall should have lead the chart. I was not the only person who noticed something was up with the data and many people raised questions about the visualization, so the poster decided to delete the post entirely. I got curious about how they may have messed up, and thankfully they included their [datasource](https://www.kaggle.com/datasets/christinezinkand/us-billiondollar-weather-and-climate-disasters), so I decided to investigate to see where they went wrong.

![](https://github.com/ryanlonergan/miniprojects/blob/main/storm_damage_viz/images/wrong_storm_damage_viz.png)

*Screenshot of the original visualization*

Before investigating, I wanted to list out a few areas where I think the original poster may have gone wrong before investigating fully. They may be incorrect, but these were the areas I wanted to investigate as starting points:

- The poster may be from the southern hemisphere and may have mixed up the months for seasons in the northern hemisphere.
- Season start and ends change depending on whether a meteorologic or calendar definition is used, which may influence the data.
- The datasource has a strange format for dates and the original poster stated that they used Excel and SQL to handle the cleaning and aggregation. I don't believe those are the ideal tools to process the data, so I'm wondering if there may have been some mistakes interpreting the dates.