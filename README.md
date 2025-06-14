# Amazon Sales EDA Analysis

![Amazon Logo](images/0_amazon_logo.jpg)

# Summary
This project performs an exploratory data analysis (EDA) on Amazon sales data, focusing on product reviews and their impact on sales performance. The analysis includes visualizations and statistical insights related to product categories, pricing, and customer ratings.

# Key Insights
1. The "Rating Histogram" graph shows that most of the reviews are between 4.0 and 4.5:
![Rating Histogram](images/1_rating_histogram.jpg)

2. I created a column to categorize the rating numbers into rating descriptions in a particular way:
* 1 to 2 -> 'Terrible'
* 2 to 3 -> 'Poor'
* 3 to 4 -> 'Average'
* 4 to 5 -> 'Good'

With this approach, I have 928 reviews classified as "Good" (63.5%), 525 as "Average" (35.9%), 8 as "Poor" (0.5%), and 1 as "Terrible" (0.1%):
![Number of Rating per Rate Description](images/2_number_of_ratings_per_rate_description.jpg)

3. I created a new column, "Macro Category" to identify the number of products evaluated per "Macro Category". We can see that the most evaluated categories are "Electronics" with 526 (36.0%), "Computers&Accessories" with 451 (30.8%), and "Home&Kitchen" with 447 (30.6%), totaling 97.8% of the overall evaluations:
![Most Evalueted Products per Macro Category](images/3_most_evalueted_products_per_macro_category.jpg)

4. This graph shows the top 10 average ratings per "Macro Category", where we can see that the first three evaluated products in the previous graph ("Electronics", "Computers&Accessories" and "Home&Kitchen") have an average rating between 4.0 and 4.2. In addition, the two best-rated products ("OfficeProducts" and "Toys&Games" have only 31 and 1 evaluations, respectively, in the previous graph:
![Average Rating per Macro Category](images/4_rating_average_per_macro_category.jpg)

5. I created a new column "Micro Category". Since there were many different micro categories, I decided to analyze only the top 10 most evaluated products within "Micro Category":

![Top 10 Evalueted Products per Micro Category](images/5_top_10_evalueted_products_per_micro_category.jpg)

6. This graph shows the top 5 and bottom 5 average ratings per "Micro Category", where we can identify that all the top 10 evaluated products in the previous graph aren't included in the top 5 best-rated products in this graph. In addition, we can see the worst-rated products in "Micro Categories" which have ratings between 3.3 and 3.6, classified as "Average" in the "Rating Description":
![Rating Average per Micro Category (Top 5 and bottom 5](images/6_rating_average_per_micro_category_top_5_and_bottom_5.jpg)

# Conclusion
This analysis highlights how customer reviews—particularly ratings—can provide valuable insights for business decisions. The majority of products are rated positively, with over 63% classified as “Good” and less than 1% as “Poor” or “Terrible,” indicating a generally satisfied customer base. However, deeper analysis reveals disparities between popularity and perceived quality: the most evaluated "Macro Categories" such as "OfficeProducts", "Electronics" and "Home&Kitchen" do not necessarily have the highest average ratings.

Moreover, within the "Micro Categories," the most reviewed products are not among the top-rated, suggesting that high sales volume does not always align with customer satisfaction. These insights underscore the importance of monitoring product ratings not just at a high level but also within specific categories, helping businesses better tailor their marketing strategies, optimize product offerings, and enhance inventory planning.

In summary, leveraging EDA techniques to dissect review data enables data-driven decisions that can improve customer experience and drive sales performance on platforms like Amazon.

# Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

# How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/felipe-lemos-costa/Amazon-Sales-EDA-Analysis.git
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Open and run the Jupyter Notebook:
   ```bash
   jupyter notebook Amazon-Sales-EDA-Analysis.ipynb
   ```

# License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
