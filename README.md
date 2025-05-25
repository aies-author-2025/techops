# TechOps

## Introduction

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

## Website

See [the TechOps website](https://aies-author-2025.github.io/techops/) to dive in deeper and/or explore our templates
and examples.

## Getting Started

Developing TechOps documentation is easy, it's just markdown!

Our research and offering focuses on content and we generally consider this work rendering and integration agnostic.  
However, for those working on teams or at companies that do not already have documentation rendering and integration standards,
we provide an example here for how documentation can be rendered cleanly making it highly accessible to a wide variety
of personas. Specifically, we offer a rendering method designed to solve the documentation overload problem 
by rendering it in a way that allows documentation users to dive deep into sections they care about, 
without losing site of the big picture. 

To render your own documentation, you can use this repo with the following steps:

1. First ensure that you have a python development environment (this you'll need to Google and follow different steps
   depending on your operating system and development needs).  Our system is tested with Python 3.12 and later, but it
   likely works with any Python version >=3.5. 
2. Install the development requirements (mainly mkdocs)

   ```bash
   pip install ".[dev]"
   ```

3. [Optional] Install the pre-commit hooks (they ensure things like yaml and md files are linked and do not 
   contain errors)

   ```bash
   pre-commit install -t pre-commit -t pre-push
   ```

4. Render your documentation

   ```bash
   mkdocs serve
   ```

Running the last command `mkdocs serve` in this folder will render a local version of our 
[TechOps Website](https://aies-author-2025.github.io/techops/).  Once you are able to do this, you can fork the 
repository, update the `mkdocs.yaml` and markdown files in the `docs` folder to create your own renderable 
TechOps documentation. 
