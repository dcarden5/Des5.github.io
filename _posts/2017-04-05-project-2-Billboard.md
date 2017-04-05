![photo](/images/project-2-billboard/Billboard Headline.png)
![photo](/images/project-2-billboard/Top 100 Headline.png)

2000 was an extraordinary year for pop music, according to Billboard's Top 100.  For example, of the number of weeks to the longest climbs to number one ranking ever in Billboard history, 2000 had a third of those tracks (Lone Star's "Amazed" 31 weeks, Creed's "With Arms Wide Open" 27 weeks, Vertical Horizon's "Everything You Want" 26 weeks)+.  Destiny's Child, fronted by the future solo superstar Beyonce Knowles, had their track "Independent Women Part 1" last the most consecutive weeks at #1 in 2000 with 11 weeks.  Santana's "Maria, Maria" also lasted 10 weeks at #1, as well.

As I began to pour over this Billboard Top 100 data, that contained tracks entering the list from June 1999 through the end of December 2000, I began to wonder the question of the pace in which tracks rose or peaked.  More specifically, is there a difference between the pace in which a track peaked, relative to when it entered the Hot 100 list. Finally, what about the pace of tracks that made it to #1 throughout this year and a half versus the cohort that did not make it to the number one ranking.  

These data contained year, artist, track (title), time (song duration), genre, date (track) entered (the Billboard Top 100), date (track) peaked (on the list), week 1 (with rankings, starting June 5, 1999) through week 76 (ending December 30, 2000).  There were several iteration of data cleaning and data preparation.  Those methodologies are briefly included here, but I encourage you to find the link in my Github account to the Jupyter notebook for more finer details.  Data cleansing included: changing variables to time format, removing extraneous characters, replacing Nan (nulls) with zeros and renaming headers.  Other methodologies included creating counters to feature engineer a flag that flagged a track as ever having reached #1 for the time duration decribed above.  Other feature creation included determining an interger to denote the difference between the date the track peaked minus the date the track entered the Top 100.

The goal of the data cleanup, exploratory data analysis and feature engineering was to perform a hypothesis tes, where my null hypothesis is that there is no difference between pace of a chart topping track and the pace of a non-chart topping track.  Consequently, the alternative hypothesis is that there is a difference between the pace a chart topping track peaked versus those non-chart toppping tracks.  Unfortunately, the sample size of the chart topping tracks is 17 and smaller than I would have wanted, however I performed the hypothesis test by calculating the p-value and t-statistic for the two-tail test and by using a confidence interval of 0.05.  I used python stats model and also calculating the same stats parametrically.

![photo](/images/project-2-billboard/Histogram All Tracks for Top 100 2001.png)

Conclusion to my hypothesis test is to reject the null hypothesis that the pace that a chart topping track peaked is the same as the pace that a non-chart topper peaked.  In other words, since the p-value of 0.02 is less than the selected confidence interval (alpha) of 0.05, then we can reject the null hypothesis. T-statistic of 0.04 is also less than the confidence interval.  Although the p-value or probability of getting the mean of x given our sample, does lend evidence to the mean date difference not being the same between those tracks that reached the one ranking and those that did not, further studies are indeed required.  Hypothesis testing will not give me magnitude of the supported difference.  

![photo](/images/project-2-billboard/Histogram Ever #1 Tracks Billboard Top 100.png)

As an additional step to attempt to convince myself that my results were not just simply due to luck of chance, I also  reshuffled the date difference (between date peaked and date entered) values 10,000 times and compared those results against the mean differences between my two cohorts. What I found is that the answer in this case is under 0.001. That is less than 0.1%. So I conclude that the difference between the averages of the samples is real.

To my surprise, the pace a non-chart topping track reached its highest rank, on average, was doubly as fast as the pace it took a chart topper to reach the best ranking.  Although one need to consider the small sample size of chart toppers, I would have imagined chart topping songs would have had a quicker rise to the top ranking.
























+ https://en.wikipedia.org/wiki/List_of_Billboard_Hot_100_chart_achievements_and_milestones