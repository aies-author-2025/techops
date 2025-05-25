# Home

## TechOps Introduction

* Are you looking for guidance on how to provide technical documentation for your AI/ML system 
  and/or its constituent models and datasets?  
* Should such documentation provide value for a wide variety of user personas 
  (e.g. managers, system users, developers, researchers, etc.)?
* Does your AI/ML system need to comply with the EU AI Act, or are you developing a model or dataset that
  you want to be used as part of an AI/ML system that needs to comply with the EU AI Act?

If you answered yes to any of these questions, TechOps is for you.  

TechOps is a set of documentation templates and examples designed to help document AI/ML application, model, and
dataset teams document and rendering their documentation in an easy-to-read manner such that any documentation 
user can quickly drill down to find the information they need without losing track of the big picture. 
TechOps is also the first set of documentation templates that we know of to completely map its sections to the 
EU AI Act, for developers and providers that need to comply with this regulation that first came into force in 
August 2024.

This work accompanies a (currently anonymous) submission to AIES 2025.

These templates and examples are not to be used before publication and serve, for the moment, 
only to demonstrate the work described in the paper. All rights reserved.

## Templates

TechOps are three separate templates for sufficiently documenting AI systems for proof of compliance with the AI Act.
The documentation is split into three levels:

* AI System documentation
* Model documentation
* Data documentation

to allow the owners of data, models, and AI systems to each maintain ownership of their own level of documentation.  
Thus, model and dataset owners whom may or may not have curated their models and datasets with a specific AI Systems in 
mind, may still create documentation contributions that the AI System documentation can reference.

These templates are meant to guide responsible stakeholders to document AI systems across various fields. 
Unlike existing lengthy and abstract questionnaires, these templates offer clear guidance for the documentation of the 
relevant processes across the AI lifecycle, translating complex requirements such as fairness and data governance 
into actionable metrics and measurable criteria that can be implemented and tracked. 
This process ensures that the abstract legal requirements of the AI Act are operationalized into concrete actions, 
making them manageable and measurable.

Following the TechOps approach also provides stakeholders comprehensive oversight on the data, model and application lifecycle. These templates track the system’s status over the 
entire AI lifecycle, ensuring traceability, reproducibility, in addition to compliance with the AI Act. 

Clear documentation also promotes discoverability, collaboration, and risk assessment.

## Examples

The templates are tested on real-world scenarios providing examples that further guide their implementation:

|                                                                            | Description                                                                                                                                                     | 
|----------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Application Documentation Example](example-application-documentation-safesite-ai.md) | SafeSiteAI is a **fictional** high-risk AI system developed to detect and monitor construction worker safety using real-time video analytics and sensor fusion. | 
| [Model Documentation Example](example-model-documentation-alisnet.md)      | A neural network for segmenting human silhouettes in photos                                                                                                     |
| [Data Documentation Example](example-data-documentation-voc-skin-tones.md) | A skin tones dataset created to support fairness evaluations of downstream computer vision models and human centric applications like SafeSiteAI                |

## How To Use

Developing TechOps documentation is easy, it's just markdown!

Our research and offering focuses on content and we generally consider this work rendering and integration agnostic.  
However, for those working on teams or at companies that do not already have documentation rendering and integration standards,
we provide an example here for how documentation can be rendered cleanly making it highly accessible to a wide variety
of personas. Specifically, we offer a rendering method designed to solve the documentation overload problem 
by rendering it in a way that allows documentation users to dive deep into sections they care about, 
without losing site of the big picture. 

See our [GitHub repository](https://github.com/aies-author-2025/techops/?tab=readme-ov-file#getting-started) 
on documentation development and rendering.
