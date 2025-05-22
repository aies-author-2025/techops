# Model Documentation Template
<!-- info: Replace with model name -->
>Info on Article 11 (paragraph 1): The AI Act requires a description of  (a) the intended puprose, version and provider, (c), (b) a description of how the system interacts with software and hardware must be included, (c) relevant versions and updates
as well as (d) all the forms in which the AI system is put into service. The overview part should point out (e) the hardware on which the system is intended to run and (f) if the system is part of the safety component of a product, (g) a basic description of the user interface and (h) the instructions for use for the deployers.
 

## Overview (Article 11, paragraph 1)
> info: This section enables all stakeholders to have a glimpse into the model selction, design and development processes. You can use this session to provide transparency to users and high level information to all relevant stakeholders. 
### Model Type
**Model Type:** (e.g., Neural Networks, Decision Trees, etc.)

### Model Description (Article 11, paragraph 1 (a))
* Description
<!-- info: Brief (max 200 words) description of the model architecture and the task(s) it was trained to solve. -->

### Status 
<!-- scope: telescope -->
<!-- info: Select **one:** -->
**Status Date:** YYYY-MM-DD

**Status:** _specify one of_:

* **Under Preparation** -- The model is still under active development and is not yet ready for use due to active "dev" updates.
* **Regularly Updated** -- New versions of the model have been or will continue to be made available.
* **Actively Maintained** -- No new versions will be made available, but this model will be actively maintained.
* **Limited Maintenance** -- The model will not be updated, but any technical issues will be addressed.
* **Deprecated** -- This model is obsolete or is no longer being maintained.

### Relevant Links
<!-- info: User studies show document users find quick access to relevant artefacts like papers, model demos, etc..
very useful. -->

Example references:

- GitHub Repository
- Paper/Documentation Link
- Initiative Demo
- Conference Talk
- API Link

### Developers
- **Name, Team**
- **Name, Team**

### Owner
<!-- info: Remember to reference developers and owners emails. -->
- **Team Name, Contact Person**

## Version Details and Artifacts (Article 11, paragraph 1(c))
<!-- scope: periscope -->
<!-- info: Provide details about the current model version
and which model version the current model card corresponds to.

For models without version number, use "Not currently tracked"
but be sure to track the release date of the model.
-->


**Current Model Version:**

**Model Version Release Date:**

**Model Version at last Model Documentation Update:**

**Artifacts:**


- Model weights (e.g. S3 bucket path)
- Model config (e.g. S3 bucket path)

## Intended and Known Usage
### Intended Use
<!-- info: This section focuses on the initial purpose and/or reasoning
for creating the model. It is important to define this section as 


Example Use Case: A university research team develops a machine learning model to predict the likelihood of hospital readmission among diabetic patients over the age of 65, using data from a regional healthcare network. The model is trained and validated specifically on this elderly population and is intended to support hospital planning and academic research. However, the team does not document the model’s intended use or demographic limitations. A health-tech company later integrates the model into a mobile app aimed at helping diabetes patients of all ages manage their care. The model performs poorly for younger users, frequently overestimating their risk of readmission. This leads to unnecessary anxiety, inappropriate self-care decisions, and false alerts to care providers. The misapplication draws criticism for lacking transparency, and regulators question the ethics of deploying a model outside its original context.   -->

* Description

### Domain(s) of use
* Description

**Specific tasks performed:**

### Out Of Scope Uses
Provide potential applications and/or use cases for which use of the model is not suitable.

### Known Applications (Article 11, 1(f))
<!-- info: Fill out the following section if the model has any
current known usages.
-->

| **Application**   | **Purpose of Model Usage**                                                 | **[AI Act Risk](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)** |
|-------------------|----------------------------------------------------------------------------|----------------------------------------------------------------------------------------------|
| [Application 1]() | Foundation model providing customer embeddings for fraud detection scoring | High                                                                                         |
| [Application 2]() | Customer embeddings used directly as features for recommendation engine    | Limited                                                                                      |

Note, this table may not be exhaustive.  Model users and documentation consumers at large
are highly encouraged to contribute known usages.

## Model Architecture (Article 11 paragraph 2 b, c)

> Info AI Act requirements: This section should contain a description of the elements of the model and the processes of its training and development. Article 11, 2(b) requires the design specifications of a system, model selection and ehat the system is designed to optimize for as well as potential trade-offs. Article 11, 2(c) a description of the systems architecture is required, how software components are build on or feed into each other and the computational resources needed to develop, train, test and validate the systems. 

<!-- Info: Describing the architecture is fundamental for reproducibility, transparency, and effective maintenance. Without clear records of the model’s layers, activation functions, input/output shapes, and training configurations, it becomes difficult to reproduce results, debug issues, or update the model reliably.  -->


- Architecture Description

- Key components
    
- Hyperparameter tuning methodology

- Training Methodology

- Training duration
    
- Compute resources used
    

### Data Collection and Preprocessing (Article 11, paragraph 2 d)

<!--check data documentation to avoid duplicates of information and link it in this sectiion

In Article 11, 2 (d) a datasheet is required which describes all training methodologies and techniques as well as the charatcteristics of the training dataset, general description of the dataset, information about their provenance, scope and main characteristics, how the data was obtained and selected labelling procedures conducted and data cleaning methodologies deployed -->

- **Steps Involved**:
    - Data collection: Describe how the data was sourced (e.g., databases, APIs, sensors, or publicly available datasets).
    - Data cleaning: Explain techniques used to handle missing values, outliers, or errors.
        
    - Data transformation: Include any scaling or encoding applied.


       
### Data Splitting 

* **Subset Definitions**:
    * **Training set**: 
    * **Validation set**: 
    * **Test set**: 
* **Splitting Methodology**:
    * Describe the approach:
        * **Random Sampling**: 
        * **Stratified Sampling**: 
        * **Temporal Splits**: 
* **Proportions**:
    * Example: "70% training, 20% validation, 10% testing."
* **Reproducibility**:
    * Mention how many seeds are being used and how many are needed to prove statistical significance
    
**Data Shuffling**:

- Shuffle applied: (Yes/No) 

## Model Training Process (Article 11, paragraph 2 (c, g), paragraph 3)

> AI Act requirements info: In Article 11 paragraph 2 c details about the computational resources needed to develop, tain, test and validate AI systems are required. Moreover, in this section, in accordance to Article 11, paragraph 2 (g) the validation and testing procedures used as well as the data and the main metrics adopted to measure accuracy, robustness, compliance with the requirements layed out in Chapter III Section 2. Paragraph 3 requires detailed information about the monitoring and fucntioning and control of the system as well as logging of testing reporting dated and signed by responsible stakeholders. 

**Details of Processes**:

- **Initialisation**: 
- **Loss Function**:
- **Optimiser**:
- **Hyperparameters**:
        
## Model Training and Validation (Article 11, paragraph 2(g)):

Objective: Clarify what the model is supposed to achieve. 

- Problem statement (e.g., classification of X, prediction of Y)
- Business goals (accuracy, fairness, speed)
- Metrics selected (e.g., accuracy, precision, recall, F1-score, AUC-ROC, MAE, RMSE)
Rationale for each metric (why accuracy? why F1-score?)

- Model predictions on the validation set evalutaion description. 

<!--
- Performance metrics (e.g., accuracy, F1 score, RMSE) are monitored.
- Documeting this step is important as it enables to detect errors and performance issues early on: Overfitting can be detected using validation loss trends.
-->

<!--### Performance Metrics

- Evaluation Metrics Used (e.g., Accuracy, Precision, Recall, AUC-ROC)
- Benchmarking Results
- Validation Process
- Real-World Performance
- Stress testing
- Performance across different environments and populations -->

**Hyperparameter Tuning**:
    

        
**Regularisation**:
    

    
**Early Stopping**:
    

## Model Testing and Evaluation

<!--
- Performance metrics (e.g., accuracy, F1 score, RMSE) are monitored.
- Documeting this step is important as it enables to detect errors and performance issues early on: Overfitting can be detected using validation loss trends.
-->
 **Performance Metrics**:
    
 - Compute metrics on the test set:
     - Accuracy, precision, recall, F1 score for classification.
    - MSE, RMSE, MAE for regression.

 **Confusion Matrix**:
    
- Generate a confusion matrix to evaluate classification results.

 **ROC Curve and AUC**:
    
- For binary classifiers, compute the ROC curve and Area Under the Curve (AUC).

 **Feature Importance**:
    
- Analyse feature contributions (for explainability).

 **Robustness Testing**:

- Test the model on edge cases or adversarial examples.

 **Comparison to Baselines**:
    
- Compare the model’s performance to a simple baseline (e.g., random guess, mean prediction).

### Model Bias and Fairness Analysis (Article 11, paragraph 2 g, f, paragraph 3, 4)

> This section aims to cover the AI Act requirements layed out in Article 11 paragraph 2 g that requires the description of the potential discriminatory impacts. 
Paragraphg 4 requires the assessment of the appropriateness of the performance metrics.  



![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXclauxwg1nWuPj2z0TcgUK9y69AqHzk_-jQ5BJwYeDkjPSOLVddFcHJ6-oOiuZ2p4Rk3VpqyKw9CvU7N1LOqYtpdjN6CV_hhTxTtpNj4auLmqhsaIQ5fRLIPnVpZOnhtR63YNELlg?key=Lv0_1kRp5_LSkJabUJ8gjQ)Implicit Bias, Measurement Bias, Temporal Bias, Selection Bias, Confounding Bias

#### Bias Detection Methods Used
    

**Pre-processing:** Resampling, Reweighting,Transformation (data imputation, changing order of data); Relabeling, Blinding
    
**In-processing:** Transfer learning, Reweighting, Constraint optimization, Adversarial Learning, Regularization, Bandits
    
**Post-processing:** Transformation, Calibration, Thresholding
    


**Results of Bias Testing:**
    

#### Mitigation Measures
    

**Fairness adjustments:** Introduce fairness criteria (like demographic parity, equal opportunity, or equalized odds) into the model training process. 
    
**Adversarial Debiasing:** Use adversarial networks to remove biased information during training. The main model tries to make accurate predictions, while an adversary network tries to predict sensitive attributes from the model's predictions.
    

#### Retraining approaches

**Fairness Regularization:** Modify the model's objective function to penalize bias. This introduces regularization terms that discourage the model from making predictions that disproportionately affect certain groups.
    
**Fair Representation Learning:** Learn latent representations of the input data that remove sensitive attributes, ensuring that downstream models trained on these representations are fair.
    
### Post-Processing Techniques

**Fairness-Aware Recalibration:** After the model is trained, adjust decision thresholds separately for different demographic groups to reduce disparities in false positive/false negative rates.
    
**Output Perturbation:** Introduce randomness or noise to model predictions to make outcomes more equitable across groups.
    
**Fairness Impact Statement:** Explain trade-offs made to satisfy certain fairness criterias
    

## Model Interpretability and Explainability (Article 11, paragraph 2 (e))
**Explainability Techniques Used:**
  <!-- for example: Shapley values, LIME, etc. Both SHAP and LIME are explainability techniques that help to understand why a machine learning model made a specific prediction — especially when the model is a complex "black box" like a random forest, gradient boosting, or deep neural net. Shap Uses game theory to assign each feature a value showing how much it contributed to a prediction. Lime biulds a simple, interpretable model (like a linear model) near the point of interest to explain the prediction -->
    
    Examples: 
    SHAP (SHapley Additive exPlanations), 
    LIME (Local Interpretable Model-agnostic Explanations)

**Post-hoc Explanation Models**

- Feature Importance, Permutation Importance, SHAP (SHapley Additive exPlanations), LIME (Local Interpretable Model-agnostic Explanations):
- Partial Dependence Plots (PDP) 
- Counterfactual Explanations
- Surrogate Models
- Attention Mechanisms (for Deep Learning)
    

**Model-Specific Explanation Techniques**

<!-- info: this part is important to delineate why a model makes a decision or to debug and identify if the model is focusing on the right parts of the input. Especially fundamental for models deployed in critical domains such as medical, financial and legal or law enforcement. This section can be useful to draft the user-interface section of the documentation.) -->

- Grad-CAM (Gradient-weighted Class Activation Mapping) for CNNs and RNNs: especially for computer vision applications 
- Layer-wise Relevance Propagation (LRP): Works well for CNNs, fully connected nets, and some RNNs (classification focused)
- TreeSHAP (SHAP for Decision Trees)
    

How interpretable is the model’s decision-making process? 


<!--
Some technical tools that can aid transparency include:
- Data Lineage Tools: Track the flow and transformation of data (e.g., Apache Atlas, Pachyderm).
- Explainability Libraries: SHAP, LIME, Captum, TensorFlow Explain.
- Version Control Systems: Git, DVC (Data Version Control) for datasets and models. -->

### EU Declaration of conformity (Article 47)

 <!-- when applicable and certifications are available: it requires a systems name as well as the name and address of the provider; a statement that the EU declaration of conformity referred to in Article 47 is issued under the sole responsibility of the provider; a statement that the AI system is in conformity with this Regulation and, if applicable, with any other relevant Union law that provides for the issuing of the EU declaration of conformity referred to in Article 47, Where an AI system involves the processing of personal data;  a statement that that AI system complies with Regulations (EU) 2016/679 and (EU) 2018/1725 and Directive (EU) 2016/680, reference to the harmonised standards used or any other common specification in relation to which
conformity is declared; the name and identification number of the notified body, a description of the conformity
assessment procedure performed, and identification of the certificate issued; the place and date of issue of the declaration, the name and function of the person who signed it, as well as an
indication for, or on behalf of whom, that person signed, a signature.-->

### Standards applied

<!-- Document here the standards and frameworks used-->

## Documentation Metadata
### Version
<!-- info: provide version of this document, if applicable (dates might also be useful) -->

### Template Version
<!-- info: link to model documentation template (i.e. could be a GitHub link) -->

### Documentation Authors
<!-- info: Give documentation authors credit

Select one or more roles per author and reference author's
emails to ease communication and add transparency. -->

- **Name, Team:** (Owner / Contributor / Manager)
- **Name, Team:** (Owner / Contributor / Manager)
- **Name, Team:** (Owner / Contributor / Manager)