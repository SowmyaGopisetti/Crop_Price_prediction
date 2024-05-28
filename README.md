# Crop_Price_prediction
The dataset is with the following features: State, Crop, CostCultivation, CostCultivation2, Production, Yield, Temperature, RainFallAnnual, and Price (target variable). Since the target is already present in the dataset, this is a supervised learning task, and because the target feature is continuous, the prediction is done using regression models.

In this project, I predicted the price using three models: Linear Regression, Support Vector Regression, and Decision Tree Regression. Their R2 scores and mean square errors were compared to evaluate performance.

𝐏𝐫𝐨𝐣𝐞𝐜𝐭 𝐖𝐨𝐫𝐤𝐟𝐥𝐨𝐰:

𝐄𝐱𝐩𝐥𝐨𝐫𝐚𝐭𝐨𝐫𝐲 𝐃𝐚𝐭𝐚 𝐀𝐧𝐚𝐥𝐲𝐬𝐢𝐬 (𝐄𝐃𝐀):

This is done to get a better understanding of the data which involved checking for null values, checking the shape of the data and checking for duplicates. I checked for the collinearity among the features by visualizing a scatter pair plot among the continuous features. My observation revealed that CostCultivation and CostCultivation2 were collinear as the scatter plot was linear between them. So, to handle that I used a feature engineering technique by making a new column CostCultivation_product which is the product of CostCultivation and CostCultivation2.

𝐃𝐚𝐭𝐚 𝐓𝐫𝐚𝐧𝐬𝐟𝐨𝐫𝐦𝐚𝐭𝐢𝐨𝐧:

Plotted histograms for continuous features and applied log transformation to those not normally distributed.

Used boxplots to detect and handle outliers.

Data Preparation:

Split the dataset into X (features) and Y (target variable).

Further, split the data into training (80%) and testing (20%) sets, resulting in X_train, X_test, Y_train, and Y_test.


𝐌𝐨𝐝𝐞𝐥 𝐓𝐫𝐚𝐢𝐧𝐢𝐧𝐠 𝐚𝐧𝐝 𝐄𝐯𝐚𝐥𝐮𝐚𝐭𝐢𝐨𝐧:

Trained and evaluated Linear Regression, Support Vector Regression, and Decision Tree Regression models and Compared models using R² scores and mean square errors.


𝐑𝐞𝐬𝐮𝐥𝐭𝐬:

Linear Regression: R² Score: 0.99

Support Vector Regression: R² Score: 0.99

Decision Tree Regression: R² Score: 0.98
