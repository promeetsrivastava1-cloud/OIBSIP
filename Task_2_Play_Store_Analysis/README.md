# Google Play Store Analysis — Data Analytics Internship

## Objective
To identify key factors driving app success (Installs/Ratings) and provide actionable insights for developers.

## Executive Summary
This analysis was performed on the Google Play Store dataset to extract actionable business intelligence. The dataset required significant cleaning, particularly regarding string-to-numeric conversions. The analysis reveals that the 'Game' category dominates the market in terms of total installs, but several high-rating categories were also identified that offer better potential for customer satisfaction over raw volume.

## Business Questions
- **Market Reach:** Which app categories have the highest "viral potential" (total installs), and how does category choice impact market penetration?
- **Quality Standards:** What is the average user satisfaction level across the store, and is there a "rating standard" that apps must meet to remain competitive?
- **Monetization Strategy:** How does the "Free vs. Paid" model affect app visibility, and are paid apps actually delivering higher value to users?
- **Engagement Drivers:** Is there a correlation between user engagement (number of reviews) and total reach (total installs), and what does this imply for marketing strategy?

## Dataset
- `googleplaystore.csv`
- `googleplaystore_user_reviews.csv`

## Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Data Cleaning & Pre-processing
- The 'Installs' column contained non-numeric characters like '+' and ',', which made it impossible to analyze mathematically. These characters were stripped and the column was converted to numeric type.
- Fixed a rating outlier issue by filtering out invalid ratings above 5 before filling missing 'Rating' values with the median.
- Converted the 'Reviews' column to numeric type.
- Removed duplicate records.

## Analysis & Insights

**Category Analysis:** The category analysis shows that the Game category leads in total installations. This suggests that developers targeting the mass market should prioritize this niche, while categories with lower installs but higher average ratings may represent more specialized, premium app opportunities.

**Distribution of App Ratings:** Most apps are rated between 4.0 and 4.5, indicating a high standard of quality across the Play Store, though there is a clear bias toward positive ratings.

**Free vs. Paid:** The vast majority of apps are free, confirming that the ad-supported and in-app-purchase models are the dominant strategies for market penetration.

**Engagement vs. Reach:** There is a clear positive correlation between the number of reviews and total installs, proving that user engagement and social proof are critical drivers for app downloads. The calculated Pearson correlation coefficient is **0.63**, indicating a moderate-to-strong positive relationship. This statistically validates that app visibility is heavily influenced by social proof; as user engagement (reviews) increases, the likelihood of higher installation volume also significantly increases. This suggests that a key part of marketing strategy should be to incentivize existing users to leave reviews.

**User Sentiment:** The sentiment distribution reveals a clear trend: the majority of user feedback is positive, which is a sign of overall app health. However, there is also a notable volume of negative sentiment. This isn't just "bad data" — it is a goldmine. Product teams should perform a sentiment-based audit, specifically filtering for the 'Negative' category to extract recurring keywords, allowing a move from passive observation to active product improvement, addressing the exact pain points that trigger user frustration.

## Final Conclusion & Actionable Recommendations

Through this comprehensive exploratory data analysis, the performance landscape of the Google Play Store was mapped out. By cleaning the dataset and analyzing the relationships between categories, ratings, and user engagement, raw data was transformed into a clear strategic overview of the mobile app market.

**Actionable Business Recommendations:**

- **Focus on High-Reach Categories:** The analysis confirms that Game and Family categories dominate total installations. Developers aiming for mass-market penetration should prioritize these genres, while those seeking premium, high-value users should investigate categories that maintain high ratings despite lower volume.
- **Leverage Social Proof:** Since there is a strong positive correlation between the number of reviews and total installs, developers should implement proactive review-prompting strategies within their apps to boost credibility and attract new users.
- **Optimise Monetisation:** Given that the vast majority of apps are free, developers should rely on in-app purchases and ad-revenue strategies rather than upfront pricing to maximize reach. If a paid model is chosen, it must be supported by premium content to justify the cost, as price-sensitive users are highly prevalent.
- **Quality First:** Because the bulk of apps are rated between 4.0 and 4.5, high quality is the "entry price" to the market. Apps falling below a 4.0 rating should undergo an immediate user-experience audit to identify and resolve performance issues that may be suppressing growth.
- **Future Work:** This analysis provides a solid baseline. Future iterations could incorporate a time-series analysis to evaluate how app updates or version changes directly correlate with sentiment shifts and rating stability over time.

- ## 🎥 Project Demonstration
You can watch the full project walkthrough and read the post here:
[**View the Post on LinkedIn**](https://www.linkedin.com/posts/promeetsrivastava_oasisinfobyte-oibsip-dataanalytics-ugcPost-7485259396705427456-3fqs/?utm_source=share&utm_medium=member_desktop&rcm=ACoAADczoOcBGCknx21-xvuTJ3EdsTSnSaYeWF0)

## Author
Promeet Srivastava
Data Analytics Intern — Oasis Infobyte
