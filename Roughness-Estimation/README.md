# Road-Roughness-Estimation

# Requirements 
1. Fastai 0.7

# STEPS
1. Load data file (df=pd.read_csv('traindata1.csv'))
2. Define your categorical and continuous variables
	cat_vars = ['speed']
	contin_vars = ['dominant_freq', 'strength','auc','sum','iri_18']
3. Apply numerical codes to your categorical variables. 
	for v in cat_vars: joined[v] = joined[v].astype('category').cat.as_ordered()
	apply_cats(joined_test, joined)
4. Use the PROC_DF fuction in fastai to process your data.
5. Split data into training and validataion  
6. Build a model using '.get_learner'.
