---


---

<h1 id="sparkify-capstone-project">Sparkify Capstone Project</h1>
<h2 id="project-description">Project Description</h2>
<p>Sparkify is a fictious music streaming app, which contains two months of user behavior log in which few users have churned out and it is essential to know which users will churn out in future and make corrective actions to retain them. This is the main motivation of this Project.</p>
<p><strong>Data</strong><br>
Only a small sample of the data is stored on the data folder as github prevents storage of file size beyond 100 MB.</p>
<p><strong>Code</strong></p>
<ul>
<li>Sparkify_Capstone_Project- Part1.ipynb - Loading &amp; Exploration of the input data</li>
<li>data_processing.py - Deals with transformation, cleaning &amp; feature extraction</li>
<li><a href="http://Modeling.py">Modeling.py</a> - Deals with modeling on the engineered features along with grid search</li>
<li>Sparkify_Capstone_Project- Part 2.ipynb - Jupyter notebook to invoke the <a href="http://Modeling.py">Modeling.py</a></li>
</ul>
<p><strong>Modeling</strong></p>
<p>Since our focus is on predicting churn, I decided to use the below 3 features as labels: ChurnedInTimeBin, WillChurnInNextBin, and WillChurnSoon and applied 3 different models (Logistic Regression, Random Forest and GBM) resulting in 9 different models to see which one does a closer prediction when it comes to churn. Moreover we use AUC-PR as a evaluation criteria make a prediction to overcome class-imbalance problem. Also performed hyperparameter tuning by employing a grid search to see which parameter yields better results. Best  Models are stored on the Model folder.</p>
<p><strong>Summary</strong><br>
The given dataset has some serious class-imbalance problem and hence the best evaluation criteria would be to use Area Under the Curve Precision Recall (AUC PR). Morever, the label WillChurnSoon was significantly the best label to predict the churn while Logistic Regression was the better classifier as it accurately predicted the churn. Although the average AUC PR of Logistic Regression in comparison with GBM, was close enough but Logistic Regression out performed to be a winner in terms of run time. Average runtime for Logistic Regression was 20 mins while that of GBM was 80 mins which is 4 times longer</p>
<p><strong>Documentation</strong><br>
Detailed documentation can be found on my <a href="https://medium.com/churn-prediction-modeling-with-pyspark">blog post</a>.</p>
<p><strong>Software Requirements</strong><br>
This project uses <strong>Python 3.7.3</strong> and the standard libraries used were pyspark, pandas, matplotlib &amp; seaborn.</p>
<p><strong>Acknowledgements</strong><br>
Thanks to <a href="https://eu.udacity.com/">Udacity</a> for providing such a challenging dataset, where the learners have to get exposed to processing JSON objects and use Spark to load, clean, transform &amp; model huge dataset.</p>
<p><strong>References</strong></p>
<ol>
<li><a href="https://dl.acm.org/citation.cfm?id=114387">https://dl.acm.org/citation.cfm?id=114387</a></li>
<li><a href="https://dl.acm.org/citation.cfm?id=1143874">https://dl.acm.org/citation.cfm?id=1143874</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2017/03/imbalanced-classification-problem/">https://www.analyticsvidhya.com/blog/2017/03/imbalanced-classification-problem/</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2017/03/imbalanced-classification-problem/">https://www.analyticsvidhya.com/blog/2017/03/imbalanced-classification-problem/</a><br>
<a href="https://www.analyticsvidhya.com/blog/2017/03/imbalanced-classification-problem/">https://www.analyticsvidhya.com/blog/2017/03/imbalanced-classification-problem/</a></li>
</ol>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>

