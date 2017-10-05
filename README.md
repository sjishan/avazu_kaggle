# Avazu - Click-Through Rate Prediction

### Files:
- **Part-1 Data Exploration**. Visualizing the data to look into aspects that will help us to decide what features to pick.
- **Part-2 Feature Engineering**. Feature Ranking of Hidden Column. Subsetting the columns and apply one-hot encoding. PCA to reduce dimension.
 - **Part-3 Predictive Modeling**. Using Multi-layer Perceptron based classifier. Analyzing Performance Metrics.

Discarded - Predictive Modeling: Attempted XGBoost modeling, however parameter tuning could be very time consuming.

### A few more things that ***may*** help design a better model:

**Improving Feature Engineering:**
- **AutoEncoder**. Deep learning to reduce dimension non-linearly. 
- **Deep CTR**. Research Paper published last year which focuses on using Denoising AutoEncoder and Restricted Boltzmann Machine to feature engineer AD CTR data. https://github.com/wnzhang/deep-ctr 
- **MCA**. Multiple correspondence analysis for categorical data.
- **Feature Bagging/Merging** - Generating new feature columns based on the existing ones. For instance, app and site columns are complementary.  
- **SMOTE**. Synthetic Minority Oversampling to handle class imbalance issue.

**Improving Model:**
- Vowpal Wabbit. On-line learning for large dataset with small memory. 
- More memory. 
- Grid Search for Parameter Tuning. Time consuming. 
