Marketing Channel Effectiveness with Lasso Regression

Dataset Overview:
This dataset contains marketing spend across multiple channels and the corresponding sales achieved.
The goal is to identify which marketing channels truly drive sales.


Features:

TV_spend: Money spent on TV advertisements

radio_spend: Money spent on radio ads

social_media_spend: Spending on social media marketing (Facebook, Instagram, Twitter, etc.)

newspaper_spend: Spending on newspaper ads

billboard_spend: Spending on billboards and outdoor media

influencer_spend: Spending on influencer partnerships

email_spend: Spending on email marketing campaigns


Target:

sales_k: Sales generated (in thousands)


Scenario:
A company invests in multiple marketing channels. However, not all channels contribute equally to sales.
We want to use Lasso regression to identify the most impactful channels by shrinking weak coefficients to zero.


Methodology:

Split the dataset into training and testing sets.

Standardize features (important for Lasso).

Fit both OLS regression and Lasso regression.

Compare coefficients:

OLS assigns a coefficient to every channel, even weak ones.

Lasso shrinks weak or irrelevant channel coefficients toward zero, keeping only the most impactful ones.


Outcome:

Important channels are those with non-zero coefficients in the Lasso model.

This helps the company allocate budget more effectively to maximize sales.


<img width="855" height="538" alt="image" src="https://github.com/user-attachments/assets/3fa76054-26c4-49b8-b78f-716fb22b612e" />

