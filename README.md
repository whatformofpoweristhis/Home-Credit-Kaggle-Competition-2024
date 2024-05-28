# Home-Credit-Kaggle-Competition-2024
**Overview**: https://www.kaggle.com/competitions/home-credit-credit-risk-model-stability

**Data**: https://www.kaggle.com/competitions/home-credit-credit-risk-model-stability/data

**Leaderboard**: https://www.kaggle.com/competitions/home-credit-credit-risk-model-stability/leaderboard



## Description
The goal of this competition is to predict which clients are more likely to default on their loans. The evaluation will favor solutions that are stable over time. 


In this competition, I achieved a public leaderboard score of 0.599 and a private leaderboard score of 0.524 by using a combination of LightGBM and CatBoost models without employing any metric hacks. When I used metric hacks, my notebook reached a highest private leaderboard score of 0.591.


However, since only two submissions could be chosen for the final entry, my team missed the opportunity to achieve 5th place and ultimately won a silver medal in the competition, finishing rank **78/3883**.


![Screenshot 2024-05-28 143827](https://github.com/whatformofpoweristhis/Home-Credit-Kaggle-Competition-2024/assets/120392332/875cb5dc-d4ab-405a-bd99-4a4cda99fb83)

![Screenshot 2024-05-28 143920](https://github.com/whatformofpoweristhis/Home-Credit-Kaggle-Competition-2024/assets/120392332/6b716b5d-2f63-43bb-8137-79d2307eba13)

## Usage
**lgb model.zip, cat model.zip**:  Trained LGB and Cat models saved in joblib format. There are five LGB and Cat models each, generated through StratifiedGroupKFold cross-validation with split=5.


**lgb-train-notebook, cat-train-notebook.ipynb**:  By specifying the file paths, run these two notebooks to output the trained LGB and Cat models, as well as the feature names required for training and prediction.


**home-credit-lgb+cat without metric trick.ipynb**:  Using a combination of LGB and Cat models to predict outcomes, achieving scores of 0.524 on the public leaderboard and 0.599 on the private leaderboard, respectively.


**home-credit-lgb+cat highest score.ipynb**:  Enhance the stability of the model by utilizing a combination of LGB and Cat models and inferring the actual dates from the characteristics of the features. 


**metric simulation.ipynb**:  Simulate the leaderboard score by assuming the Weekly AUC as a linearly declining straight line.


**feature importances summary.txt**:  Overview of the importance of all features as calculated by the LGB model.





