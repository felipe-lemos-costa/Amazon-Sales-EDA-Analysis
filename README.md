# Amazon Sales EDA Analysis

![Amazon Logo](images/Amazon.jpg)

# Summary
This project performs an exploratory data analysis (EDA) on Amazon sales data, focusing on product reviews and their impact on sales performance. The analysis includes visualizations and statistical insights related to product categories, pricing, and customer ratings.

# Key Insights
1. The "Rating Histogram" graph shows that most of the reviews are between 4.0 and 4.5.
![Rating Histogram](images/rating_histogram.jpg)

2. I created a column to categorize the rating numbers into rating descriptions in a particular way:
* 1 to 2 -> 'Terrible'
* 2 to 3 -> 'Poor'
* 3 to 4 -> 'Average'
* 4 to 5 -> 'Good'
![Number of Rating per Rate Description](images/number_of_rating_per_rate_description.jpg)


# Technologies
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
