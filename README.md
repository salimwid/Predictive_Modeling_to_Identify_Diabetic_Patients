# Predictive_Modeling_to_Identify_Diabetic_Patients

### Machine Learning Models Deployed
SVC, Logistic Regression, Decision Tree Classifier, Random Forest, XGBoost

### Techniques Employed
Exploratory Data Analysis, Data Visualization, Dimension Reduction, PCA, Cross Validation, ROC Curve, Machine Learning

### Context
As of 2019, the World Health Organization (WHO) ranks diabetes as one of the top 10 leading causes of death with over 1.5 million deaths per annum globally. In the United States alone, the American Diabetes Association estimates a staggering $237 billions in direct medical costs and another $90 billions in lost productivity to diabetes1. This roughly means that 1 in every $4 healthcare dollars is spent on diabetes treatment.<br>

This project aims to create classification models that could help detect early diabetes status of individuals in the United States to reduce the costs bear by insurance companies. Currently, insurance companies commonly screen for diabetes by comparing a claimant’s Body Mass Index (BMI), Blood Glucose Level after Two Hour Oral Glucose Test (OGTT) and Glycohemoglobin level against a benchmark guideline provided by the American Diabetes Association. This method however, only identifies around 30% of diabetics. <br>

Using analytics, insurance companies can move from reactively adjusting premiums to a more active role. With the wealth of information collected during the underwriting and claims process, insurance companies can build a classification model that can:<br>
(1) Compute the probability of positive diagnosis given lifestyle & medical test variables <br>
(2) Identify high risk patients (potential pre-diabetes) for monitoring and intervention<br>
(3) Show insured clients’ current state of health relative to medical benchmarks<br>
(4) Directly identified patients to merchant partners who could help them effect required lifestyle changes to prevent, delay or alleviate the after-effects of diabetes.<br>

### Datasets
The National Health and Nutrition Examination Survey (NHANES) dataset for diabetes were used. The dataset contains information akin to what insurance firms would have access to throughout the life of the customer relationship.<br>

The original dataset consists of 4 separate tables: <br>
(a) demographics, <br>
(b) blood mineral, <br>
(c) physical examination results and <br>
(d) the diabetic/non-diabetic labels. <br>

Overall, there were over 83 original features and 10,175 individual rows, which were joined using SEQN (individual id in the dataset) into one table.

### Impact from Findings
Performance Comparison in Dollars were measured by adopting ‘Expected Claim (EC)’ framework to assess three conditions:<br>
(1) Perfect Classifier: This ideal model classifies all observations correctly. Plugging some values into the EC formula, the expected claims value would be $5,575.70. Performance will be judged based on the difference from this base value.<br>
(2) Current Method: The current standard yields an EC value of $6075.37.<br>
(3) Our Model: XGBoost run with tuned settings yields an EC value of $5,778.13.<br>

Comparing the current standard with XGBoost shows a clear 59.49% uplift ($499.67 vs $202.43 differential per head). When superimposed on top of the 2,962 test individuals, this translates to over a $800,000 impact to the company bottom line.
<br>
### Collaborators
Gino Martelli Tiu (@ginosytiu)<br>
Susan Koruthu (@skoruthu)<br>
Widya Salim (@salimwid)<br>
Xhoni Shollaj (@Xns140)<br>
