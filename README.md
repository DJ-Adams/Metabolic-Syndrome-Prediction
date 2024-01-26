# Analysis of Key Indicators in Predicting Metabolic Syndrome

<p align="center" width="100%">
  <img width="90%" src="https://jamestownspine.com/wp-content/uploads/2019/09/What-is-Metabolic-Syndrome.jpg">
</p>


 <a href="https://jamestownspine.com/metabolic-syndrome/">Image Source</a></center>

This dataset comes from a group of medical professionals who are interested in potentially isolating key indicators for Metabolic Syndrome. They have asked us to take patient medical and demographical information and discover trends that may help highlight the most important factors in predicting Metabolic Syndrome.

## Method Overview

The stakeholders provided data was cleaned, encoded and sclaled. I filled in amy missing values with the median values of each column. I tuned a Random Forest Model and isolated the most important features and permutation importances.

![importances](https://github.com/DJ-Adams/Metabolic-Syndrome-Prediction/assets/140389867/504c3c4f-b0c7-46c4-97f9-cc04f30ffb75)

During my analysis the model indicated that  Blood Glucose and Triglyceride levels were important features in Metabolic Syndrome instances.

<p align="center" width="100%">
    <img width="47%" src="https://github.com/DJ-Adams/Metabolic-Syndrome-Prediction/assets/140389867/bdd38a2c-28e6-44a2-9a5e-9bb87eeed851">
    <img width="47%" src="https://github.com/DJ-Adams/Metabolic-Syndrome-Prediction/assets/140389867/58bf6e93-756d-4d02-b57d-4592da426b27">
</p>

## Neural Network Model

I created a neural network model and tuned it by adding drop out layers and adjusting the optimizer to get the best predictive model.

![Screenshot 2024-01-26 12 55 13 AM](https://github.com/DJ-Adams/Metabolic-Syndrome-Prediction/assets/140389867/64099589-d3ab-4b14-adeb-50cf21911dd2)


## Final Metrics and Analysis

<p align="center" width="100%">
    <img width="47%" src="https://github.com/DJ-Adams/Metabolic-Syndrome-Prediction/assets/140389867/23a8ea76-a2e5-4efe-a16b-5cfb3eff9225">
    <img width="47%" src="https://github.com/DJ-Adams/Metabolic-Syndrome-Prediction/assets/140389867/ac73da90-25eb-4305-a4d1-07606b26f37f">
</p>

![Screenshot 2024-01-26 1 08 44 AM](https://github.com/DJ-Adams/Metabolic-Syndrome-Prediction/assets/140389867/0dff6626-7c47-4879-bd8d-273ca791866f)
 
![Screenshot 2024-01-26 1 01 07 AM](https://github.com/DJ-Adams/Metabolic-Syndrome-Prediction/assets/140389867/6e1d98a7-4934-40ce-8b29-e071bc30687a)
>
</p>


The preliminary tuning I performed on the neural network was not able to outperform my tuned Random Forest model.
I was able to achieve about 85% accuracy with the neural model while obtaining 87% with the Random Forest.

![Screenshot 2024-01-26 1 22 31 AM](https://github.com/DJ-Adams/Metabolic-Syndrome-Prediction/assets/140389867/761cb64b-ff05-4a50-908b-f7c97c420284)

#### Using a feature selector wrapper with the top 10 feature importances on a Random Forest Model produced the best results and isolated the important indicators for the development of Metabolic Syndrome.
