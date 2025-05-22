# Application Documentation Template

## General Information 

(Article 11, paragraph 1 and 2:https://artificialintelligenceact.eu/article/11/)
> Info: this section covers the AI Act requirement of a description of  the intended puprose, version and provider, relevant versions and updates. In Article 11, 2 (d) a datasheet is required which describes all training methodologies and techniques as well as the charatcteristics of the training dataset, general description of the dataset, information about their provenance, scope and main characteristics, how the data was obtained and selected labelling procedures conducted and data cleaning methodologies deployed.  

**Purpose and Intended Use**:
    
   - Description of the AI system's intended purpose, including the sector of deployment.
   - Clearly state the problem the AI application aims to solve.
   - Delineate target users and stakeholders.
   - Set measurable goals and key performance indicators (KPIs).
   - Consider ethical implications and regulatory constraints. 
   - Clear statement on prohibited uses or potential misuse scenarios.
   - **Operational environment:** Describe where and how the AI system will operate, such as on mobile devices, cloud platforms, or embedded systems.


## Risk classification

> info: The AI Act classifies AI systems into four different risk categories. The EU AI Act categorizes AI systems into four risk levels: unacceptable, high, limited, and minimal risk, each with corresponding regulatory requirements. Unacceptable risk (Chapter II, Article 5) includes systems that pose a clear threat to safety or fundamental rights (e.g. social scoring, recidivism scoring) and are banned.
High-risk systems include AI used in sensitive domains like healthcare, law enforcement, education, employment, and critical infrastructure. These must meet strict requirements and conduct conformity assessmrent practices , including risk management, transparency, and human oversight.
Limited-risk systems, such as chatbots, must meet transparency obligations (e.g. disclosing AI use).
Minimal-risk systems, like spam filters or AI in video games, face no specific requirements. 

- High / Limited / Minimal (in accordance with the AI Act)
- reasoning for the above classification
   
## Application Functionality 

(Article 11, paragraph 1, 2, 3: https://artificialintelligenceact.eu/article/11/)

>Info: this section covers the delineation of the genral purpose of the system required in article 1 with a focus on defining what the system should do and how it
should work. 


- **Instructions for use for deployers**:
(Article 13: https://artificialintelligenceact.eu/article/13/ )


- **Model Capabilities**:
  
    - What the application can and cannot do (limitations).
    - Supported languages, data types, or scenarios.

- **Input Data Requirements**:
    
    - Format and quality expectations for input data.
    - Examples of valid and invalid inputs.

- **Output Explanation**:
    
    - How to interpret predictions, classifications, or recommendations.
    - Uncertainty or confidence measures, if applicable.

- **System Architecture Overview**:
    
    - Functional description and architecture of the system.
    - Describe the key components of the system (including datasets, algorithms, models, etc.)

- **Data and Model Documentation integration**:
    
    - Logging of necessary data and model documentation and responsible contacts.


## Data Documentation 
(Article 11, paragraph 2 (d))

<!--In Article 11, 2 (d) a datasheet is required which describes all training methodologies and techniques as well as the charatcteristics of the training dataset, general description of the dataset, information about their provenance, scope and main characteristics, how the data was obtained and selected labelling procedures conducted and data cleaning methodologies deployed -->

**Data Collection**:
- Define the orgin of the data (existing databases, APIs, or custom collection methods).
- How does the data represent the real-world context of the application?

<!-- color code here for data documentation elements that must be checked from the responsible stakeholder to avoid duplicates in documentation that are hard to maintain>
- **Data Documentation**:
- Define the types of data the model will process (e.g., images, text, time-series).
- Document the expected size, format, and quality of training datasets.
- Specify any preprocessing steps or feature engineering needed.
   - Clean and preprocess the data (e.g., handling missing values, normalisation).
    - Annotate and label data if required (for supervised learning).
    - Split the dataset into training, validation, and test sets.
   - Training dataset details


   **Data Cleaning**:
    
    - Handling missing values, duplicates, and outliers.
- **Normalisation/Standardisation**:
    
    - Scaling data to a specific range or standard deviation.
- **Encoding**:
    
    - Converting categorical data (e.g., one-hot, label encoding).
- **Transformation**:
    
    - Applying mathematical transformations (e.g., log, square root).
- **Augmentation**:
    
    - Expanding datasets with techniques like flipping images or paraphrasing text.
- **Anonymisation**:
    
    - Masking or pseudonymising sensitive data for privacy compliance.
- **Balancing**:
    
    - Addressing imbalanced datasets (e.g., oversampling, SMOTE).
- **Feature Selection/Removal**:
    
    - Criteria for keeping or removing features.
-->

## Model Development 

(Article 11, paragraph 1 c, g, 2, 3 4: https://artificialintelligenceact.eu/article/11/, Article 15: https://artificialintelligenceact.eu/article/15/)

>Info: In Article 11 paragraph 2 c details about the computational resources needed to develop, tain, test and validate AI systems are required. Moreover, in this section, in accordance to Article 11, paragraph 2 (g) the validation and testing procedures used as well as the data and the main metrics adopted to measure accuracy, robustness, compliance with the requirements layed out in Chapter III Section 2. Paragraph 3 requires detailed information about the monitoring and fucntioning and control of the system as well as logging of testing reporting dated and signed by responsible stakeholders.  Paragraph 4 requires a description of the appropriateness of the performance metrics for the specific AI system. Defining the appropriateness of performance metrics is important to reflect the real-world costs of errors in the specific application. Without this, even technically strong models can fail their actual purpose.

 **Model Architecture**

- Describe the selected algorithms and architectures  (e.g., supervised, unsupervised, or reinforcement learning).
- **Hyperparameter Tuning Details**: List of chosen hyperparameters and their values, including justification for selection.
- **Training Logs**: Document the training process, including time, resources used, and any issues encountered (e.g., convergence).
- Describe the design and training of the model using the prepared data.
- Results of the  test and validatation the model's performance on separate datasets.
- Include diagrams or descriptions of key components and their interactions.

Refer here to the model documentation and decsribe the appropriateness of the performance metrics selected for the application of such models in a specific context

<!-- Example: In medical diagnosis, using accuracy alone can be misleading in imbalanced datasets, potentially missing critical cases like cancer. Metrics like recall (which measures the percentage of actual cancer cases the model correctly identifies. Critical for minimizing missed diagnoses), precision ( to ensure that when the model predicts cancer, it’s actually correct—important to reduce false alarms), F1 score, and AUC-ROC provide a more meaningful assessment by accounting for the real-world impact of false positives and false negatives. Choosing the right metrics ensures models are effective, trustworthy, and aligned with practical goals and consequences.




 Color code here for model documentation elements that must be checked from the responsible stakeholder to avoid duplicates in documentation that are hard to maintain>

## Model Validation and Testing
- **Assess the metrics of model performance** 
   - accuracy:
   - precision: 
   - recall:
   - F1 score:

- **Advanced performance metrics**
  - ROC-AUC:
    - trade-off between true positive rate and false positive rate
  - PR- AUC
     - Evaluating precision and recall trade-off
  - Specificity
    - (True Negatives/(True Negatives+False Positives))
  - Log Loss (Cross-Entropy Loss):
    - Penalises incorrect probabilities assigned to classes.


- **Context dependant metrics**: 
  - Regression Metrics: For tasks predicting continuous values
  - Clustering Metrics: for tasks grouping similar data points
  - Ranking Metrics: for tasks predicting rankings (e.g., search engines recommendation systems)
  - NLP processing metrics (e.g., text classification, sequence-to-sequence tasks)


- **Fairness Metrics**:
    
    - Ensure the model treats different groups (e.g., based on gender, race) equitably.
    - Examples: Demographic parity, equal opportunity, and disparate impact.
- **Explainability Metrics**:
    
    - Measure how understandable and interpretable are the model’s decisions.
    - Examples: Feature importance, fidelity (how well explanations match the model), and sparsity (using fewer features for explanations).
    - 
- **Robustness Metrics**:
    
    - Assess how well the model performs under challenging or unexpected conditions.
    - Examples: Adversarial robustness, performance under data drift, and sensitivity to input changes.
 
- Limitations of the performance after the tests
- Simulate deployment scenarios to understand real-world implications.
- Define thresholds for acceptable performance levels.
- Justify the choice of metrics based on the application’s purpose.
   
--> 


## Deployment
    
- Infrastructure and environment details (e.g., cloud setup, APIs).
- Integration with external systems or applications.



### Infrastructure and Environment Details

- **Cloud Setup**:
    - Specify cloud provider (e.g., AWS, Azure, GCP) and regions.
    - List required services: compute (e.g., EC2, Kubernetes), storage (e.g., S3, Blob Storage), and databases (e.g., DynamoDB, Firestore).
    - Define resource configurations (e.g., VM sizes, GPU/TPU requirements).
    - Network setup: VPC, subnets, and security groups.

- **APIs**:
    - API endpoints, payload structure, authentication methods (e.g., OAuth, API keys).
    - Latency and scalability expectations.


## Integration with External Systems 

(Article 11, paragraph 1 (b, c, d, g, h), 2 (a): https://artificialintelligenceact.eu/article/11/)

- **Systems**:
    - List dependencies 
    - Data flow diagrams showing interactions.
    - Error-handling mechanisms for APIs or webhooks

## Deployment Plan

- **Infrastructure**:
    
    - List environments: development, staging, production.
    - Resource scaling policies (e.g., autoscaling, redundancy).
    - Backup and recovery processes.
  
- **Integration Steps**:
    
    - Order of deployment (e.g., database migrations, model upload, service launch).
    - Dependencies like libraries, frameworks, or APIs.
    - Rollback strategies for each component.

 - **User Information**: where is this under deployment?


 ## Lifecycle Management 
 (Article 11, paragraph 6: https://artificialintelligenceact.eu/article/11/)
    
- Monitoring procedures for performance and ethical compliance.
- Versioning and change logs for model updates.

- **Metrics**:
    
    - Application performance: response time, error rate.
    - Model performance: accuracy, precision, recall.
    - Infrastructure: CPU, memory, network usage.

- **Key Activities**:

    - Monitor performance in real-world usage.
    - Identify and fix drifts, bugs, or failures.
    - Update the model periodically.
  
- **Documentation Needs**:
    - **Monitoring Logs**: Real-time data on accuracy, latency, and uptime.
    - **Incident Reports**: Record of failures, impacts, and resolutions.
    - **Retraining Logs**: Data updates and changes in performance.
    - **Audit Trails**: Comprehensive history of changes to ensure compliance.

-**Manteinance of change logs**: 
 - new features added
- updates to existing functionality
- deprecated features
-removed features
-bug fixes
- security and vulnerability fixes


### Risk Management System 

(Article 11, paragraph 5, Article 9: https://artificialintelligenceact.eu/article/11/; https://artificialintelligenceact.eu/article/9/)

<!--**Instructions:**  A thorough risk management system is mandated by the AI Act, especially for high-risk AI systems. This section documents the  proactive efforts to ensure the AI system operates safely and ethically. In general in this section you should document all the measures undertaken to make sure that a system operates safely on the market. Example: Consider a facial recognition system used for real-time law enforcement in public spaces. This is categorized as high-risk under the EU AI Act. If developers document the risk that the system might misidentify individuals—particularly among minority groups due to biased training data—they can plan for rigorous dataset audits, independent bias testing, and establish human oversight in decision-making. Without documenting this risk, the system might be deployed without safeguards, leading to wrongful detentions and legal liabilities. Systematic documentation ensures these issues are not only identified but addressed before harm occurs.-->


**Risk Assessment Methodology:** Describe the frameworks or standards used to identify and assess risks, such as ISO 31000 or failure mode and effects analysis (FMEA), or NIST Risk Assessment Framework.

**Identified Risks:** 

**Potential Harmful Outcomes:** List possible negative effects, such as biased decisions, privacy breaches, or safety hazards.

**Likelihood and Severity:** Assess how likely each risk is to occur and the potential impact on users or society.

#### Risk Mitigation Measures:

**Preventive Measures:** Detail actions taken to prevent risks, like implementing data validation checks or bias reduction techniques.

**Protective Measures:** Describe contingency plans and safeguards in place to minimize the impact if a risk materializes.

## Testing and Validation (Accuracy, Robustness, Cybersecurity)

**Testing and Validation Procedures (Accuracy):**

**Performance Metrics:** List the metrics used to evaluate the AI system, such as accuracy, precision, recall, F1 score, or mean squared error.

**Validation Results:** Summarize the outcomes of testing, including any benchmarks or thresholds met or exceeded.

**Measures for Accuracy:** High-quality data, algorithm optimisation, evaluation metrics, and real-time performance tracking.

  
#### Accuracy throughout the lifecycle:

**Data Quality and Management:** High-Quality Training Data: Data Preprocessing, techniques like normalisation, outlier removal, and feature scaling to improve data consistency, Data Augmentation, Data Validation

**Model Selection and Optimisation:** Algorithm selection suited for the problem, Hyperparameter Tuning (grid search, random search, Bayesian optimization), Performance Validation( cross-validation by splitting data into training and testing sets, using k-fold or stratified cross-validation), Evaluation Metrics (precision,recall, F1 score, accuracy, mean squared error (MSE), or area under the curve (AUC).

**Feedback Mechanisms:** Real-Time Error Tracking, Incorporate mechanisms to iteratively label and include challenging or misclassified examples for retraining.

#### Robustness 

< Add outlier detection and all possible post analysis, whr are the criticalities>

**Robustness Measures:**
- Adversarial training, stress testing, redundancy, error handling, and domain adaptation.

**Scenario-Based Testing:**
- Plan for adversarial conditions, edge cases, and unusual input scenarios.
    
- Design the system to degrade gracefully when encountering unexpected inputs.
    

**Redundancy and Fail-Safes:**
    
- Introduce fallback systems (e.g., rule-based or simpler models) to handle situations where the main AI system fails.
    
**Uncertainty Estimation:**
    
- Include mechanisms to quantify uncertainty in the model’s predictions (e.g., Bayesian networks or confidence scores).
    

#### Cybersecurity 
(Article 11, paragraph 2 h)

**Data Security:**

**Access Control:**

**Incident Response :**


These measures include threat modelling, data security, adversarial robustness, secure development practices, access control, and incident response mechanisms.

Post-deployment monitoring, patch management, and forensic logging are crucial to maintaining ongoing cybersecurity compliance.

Documentation of all cybersecurity processes and incidents is mandatory to ensure accountability and regulatory conformity.

  

## Human Oversight 
(Article 11, paragraph 2 e, Article 14)
Link: https://artificialintelligenceact.eu/article/11/; https://artificialintelligenceact.eu/article/14/)

> AI Act Article 11, paragraph 2 (e) requirements: assessment of the human oversight measures needed in accordance with Article 14, including the assessment of the technical measures needed to facilitate the integration of the outputs of the AI systems by deployers (Article 13 paragrapgh 3 (d))

**Human-in-the-Loop Mechanisms:**  Explain how human judgment is incorporated into the AI system’s decision-making process, such as requiring human approval before action.

**Override and Intervention Procedures:** Describe how users or operators can intervene or disable the AI system in case of errors or emergencies.

**User Instructions and Training:** Provide guidelines and training materials to help users understand how to operate the AI system safely and effectively.

**Limitations and Constraints of the System:** Clearly state what the AI system cannot do, including any known weaknesses or scenarios where performance may degrade.



## Incident Management
<!-- what happens when things go wrong -->
- **Common Issues**:
    
    - List common errors and their solutions.
    - Logs or debugging tips for advanced troubleshooting.

- **Support Contact**:
    
    - How to reach technical support or community forums.


### Troubleshooting AI Application Deployment

This section outlines potential issues that can arise during the deployment of an AI application, along with their causes, resolutions, and best practices for mitigation.


#### Infrastructure-Level Issues

##### Insufficient Resources
- **Problem**: Inaccurate resource estimation for production workloads.
  - Unexpected spikes in user traffic can lead to insufficient resources such as compute, memory or storage that can lead to crashes and bad performance

- **Mitigation Strategy**:
<!-- describe here the resolution strategy such as:
-  Enable autoscaling (e.g., Kubernetes Horizontal Pod Autoscaler).
  - Monitor usage metrics and adjust resource allocation dynamically.
  - Implement rate-limiting for traffic spikes. -->


##### Network Failures
- **Problem**:  network bottlenecks  can lead to inaccessible or experiences latency of the application.

- **Mitigation Strategy**:
<!-- 
  - Test network connectivity 
  - Use content delivery networks (CDNs) or regional load balancers.
  - Ensure proper failover mechanisms.-->


##### Deployment Pipeline Failures
- **Problem**: pipeline fails to build, test, or deploy because of issues of compatibility between application code and infrastructure, environment variables or credentials misconfiguration.

- **Mitigation Strategy**: 
<!--:
  - Roll back to the last stable build.
  - Fix pipeline scripts and use containerisation for environment consistency.
  - Enable verbose logging for error diagnostics.-->


#### Integration Problems

##### API Failures
- **Problem**: External APIs or internal services are unreachable due to network errors or authentication failures.

- **Mitigation Strategy**:
<!--:
  - Implement retries with exponential backoff.
  - Validate API keys or tokens and refresh as needed.
  - Log and monitor API responses for debugging. -->

##### Data Format Mismatches
- **Problem**: Crashes or errors due to unexpected data formats such as changes in the schema of external data sources or missing data validation steps.

- **Mitigation Strategy**: 

<!-->
  - Use schema validation tools (e.g., JSON schema validators).
  - Add versioning to APIs and validate inputs before processing.-->

#### Data Quality Problems
- **Problem**: Inaccurate or corrupt data leads to poor predictions.
- **Causes**:
  - No data validation or cleaning processes.
  - Inconsistent labelling in training datasets.

- **Mitigation Strategy**: 
<!--
- **Resolution**:
  - Automate data quality checks (e.g., Great Expectations framework).
  - Regularly audit and clean production data.-->


#### Model-Level Issues

#####  Performance or Deployment Issues
- **Problem**: Incorrect or inconsistent results due to data drift or inadequate training data for the real world deployment domain. 

- **Mitigation Strategy**:

<!--
- **Resolution**:
  - Monitoring for data drift and retraining of the model as needed.
  - Regularly update the model -->


#### Safety and Security Issues

##### Unauthorised Access
- **Problem**: Sensitive data or APIs are exposed due to misconfigured authentication and authorization.

##### Data Breaches
- **Problem**: User or model data is compromised due to insecure storage or lack of monitoring and logging of data access. 

- **Mitigation Strategy**: 
<!--
- **Resolution**:
  - Use secure storage services (e.g., AWS KMS).
  - Implement auditing for data access and alerts for unusual activity.
  6.1. Delayed or Missing Data-->


#### Monitoring and Logging Failures

##### Missing or Incomplete Logs
- **Problem**: Lack of information to debug issues due to inefficient logging. Critical issues go unnoticed, or too many false positives occur by lack of implementation ofactionable information in alerts. 

- **Mitigation Strategy**: 


<!--
- **Resolution**:
  - Fine-tune alerting thresholds and prioritise critical alerts.
  - Use tools like Prometheus Alertmanager to manage and group alerts. -->


#### Recovery and Rollback

##### Rollback Mechanisms
- **Problem**: New deployment introduces critical errors.

- **Mitigation Strategy**: 

<!--
- **Resolution**:
  - Use blue-green or canary deployments to minimise impact.
  - Maintain backups of previous versions and configurations. -->

##### Disaster Recovery
- **Problem**: Complete system outage or data loss.

- **Mitigation Strategy**:

<!--
- **Resolution**:
  - Test and document disaster recovery plans.
  - Use automated backups and verify restore procedures.-->

### EU Declaration of conformity 
(Article 47:https://artificialintelligenceact.eu/article/47/)

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