# Health Indexing of Distribution Transformers (DTRs) using ML-based regression algorithms
Health Indexing of Distribution Transformers (DTRs) is a critical yet often overlooked aspect in the electric utility industry. While preventive and predictive maintenance of power transformers using myriad sensors is a well-established practice, DTRs have received limited attention due to their huge fleet scattered across different areas, inadequate manpower to handle them and lack of sufficient data. This project aims to address this gap by deploying Machine Learning-based regression algorithms for the Health Indexing of DTRs. It is a significant step for any utility towards better asset management, enhancing reliability and ensuring service continuity through adverse situations. 

## Key Contributions:
- Dataset creation: I curated a dataset from scratch using CESC's (Calcutta Electric Supply Corporation) online database, studying the relationships between various DTR parameters and their impact on winding failure.
- Predictive modeling: I used ML-based regression models like Random Forest, Support Vector Regression (SVR) and XGBoost Regression to predict the failure ages of 100+ in-service DTRs of a particular district in West Bengal, India, performed Residual Life Assessment (RLA), and assigned health indices such as "prone to failure", "deteriorated", "fair", "good" and "new" based on their residual lives.
- Industrial implementation:  This project is among the first to focus on the health indexing of DTRs on an industrial scale, offering a unique and valuable contribution to the field. This will help electric power utilities monitor and maintain their numerous and scattered DTRs, which represent a substantial capital investment.

## Comparison of performance
The performance of the aforementioned algorithms have been compared based on their results on a test dataset (not included in this repo) and their corresponding R^2 values, Mean Absolute Error (MAE) and Mean Squared Error (MSE). Based on these, Random Forest was chosen to be the best-suited algorithm for this dataset (some other algorithm may be better for a different dataset).

![compare](https://github.com/anushhkaaa/Distribution-Transformer-Health-Indexing/assets/140095723/bd614459-8506-46c0-b5a2-e4ffcd117d68)                    ![r2 values](https://github.com/anushhkaaa/Distribution-Transformer-Health-Indexing/assets/140095723/fe750e0d-3316-4b7f-a4aa-a1e68c8d6173)

## Dataset
The training and the test dataset has been uploaded. The contrasting feature is that the test dataset consists of in-service DTRs whose failure ages were predicted by the model, whereas the training dataset has failed DTRs from the last three years, till June 2023. Lack of sufficient data is a contraint that 

## Future Improvements
To get better results, the dataset can be expanded to include a holistic representation of all the classes of available data to reduce data imbalance, perform better feature engineering techniques and hyper-parameter tuning to cater to a particular dataset. 


