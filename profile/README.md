# Cambio-Project

# Goal
The Cambio-Project encompasses a collection of tools designed for Chaos Engineering. Its purpose is simulating and analysing the transient behavior of a microservice systems in resilience scenarios.

## Overview

![dispel_overview](https://github.com/Cambio-Project/.github/assets/77619091/9767110d-0b95-44df-9b2c-3a52e8e32bcf)


The  DiSpel components are eight tools with different responsibilites.

| **Component** | **Short Description** |
|---------------|-----------------------|
| [TransVis frontend](https://github.com/Cambio-Project/conversational-transient-behavior-visualization-backend/tree/master) & [TransVis backend](https://github.com/Cambio-Project/conversational-transient-behavior-visualization-frontend/tree/master)  | TransVis visualizes the transient behavior (i.e. QoS over time) of a microservice system. Additionally offers a chatbot for interactive analysis. |
| [TQPropRefiner](https://github.com/Cambio-Project/transient-behavior-requirement-refiner)   | The TQPropRefiner is a tool for the refinement of the temporal ocmponent of a generic PSP. |
| [SAE Tool](https://github.com/Cambio-Project/software-architecture-extraction)   |  The SAE tool uses event traces of a microservice application to create an architectural model. |
| [TL-Tea](https://github.com/Cambio-Project/TL-Tea)   | TL-Tea parses and converts LTL and MTL patterns into tree structures, that can be evaluated and improved. |
| [PSP Wizard](https://github.com/Cambio-Project/PSPWizardExtended)   | The PSPWizard allows for the machine-assisted creation of Property Specification Patterns (PSPs). |
| [RESIRO](https://github.com/Cambio-Project/hazard-elicitation)   |  RESIRIO is a chatbot approach for helping developers to create resilience scenarios. |
| [MiSim](https://github.com/Cambio-Project/MiSim)   | MiSim simulates a microservice system with customizable capacities, loadbalancing strategies, network delays and other real-world factors. |
| [TBVerifier](https://github.com/Cambio-Project/transient-behavior-verifier)    | The TBVerifiers enables monitoring the transient behavior of a microservice system after the injection of an anomaly.

# Code Guidelines
We use comon code guideline standards for Java and Python. Additionaly we use a template for commit messages.

## Python
- PEP 8: The Style Guide for Python Code (https://pep8.org/)
- The Hitchhikers Guide to Python (https://docs.python-guide.org/writing/style/#we-are-all-responsible-users)

## Java
- Oracle: Code Conventions for the Java Programming Language (https://www.oracle.com/java/technologies/javase/codeconventions-contents.html)
- Alibaba: Java  Coding Guidelines Alibaba Java Coding Guidelines (only chapter 1+2!) (https://alibaba.github.io/Alibaba-Java-Coding-Guidelines/)

## Commits
- Conventional Commits (https://www.conventionalcommits.org/en/v1.0.0/)
- Committing Code Guidelines [CommittingCodeGuidlines.pdf](https://github.com/Cambio-Project/.github/files/13424983/CommittingCodeGuidlines.pdf)

Template
```
# Title: Summary, imperative, start upper case, don't end with a period
# No more than 50 chars. #### 50 chars is here:  #

# Remember blank line between title and body.

# Body: Explain *what* and *why* (not *how*). Include issue ID.
# Wrap at 72 chars. ################################## which is here:  #

# At the end: Include Co-authored-by for all contributors. 
# Include at least one empty line before it. Format: 
# Co-authored-by: name <user@users.noreply.github.com>
#
# How to Write a Git Commit Message:
# https://chris.beams.io/posts/git-commit/
#
# 1. Separate subject from body with a blank line
# 2. Limit the subject line to 50 characters
# 3. Capitalize the subject line
# 4. Do not end the subject line with a period
# 5. Use the imperative mood in the subject line
# 6. Wrap the body at 72 characters
# 7. Use the body to explain what and why vs. how

# Please enter the commit message for your changes. Lines starting
# with '#' will be ignored, and an empty message aborts the commit.
#
# On branch master
# Your branch is up to date with 'origin/main'.
#
# Changes to be committed:
#       new file:   installation.md
```

