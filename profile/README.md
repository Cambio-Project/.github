# Cambio-Project

# Goal
The Cambio-Project encompasses a collection of (mostly standalone) tools designed for Chaos Engineering. Its purpose is simulating and analyzing the transient behavior of a microservice systems in resilience scenarios. Some of these tools have been integrated into a Chaos Engineering approach called *DiSpel Approach* which is detailed in the following.

## Overview

<img width="960" alt="dispeloverview" src="https://github.com/Cambio-Project/.github/assets/18191871/1131d3b4-c1f5-4185-b2bc-33d8225c5f30">

The **DiSpel components** are currently six tools with different responsibilites.

| **Component** | **Short Description** |
|---------------|-----------------------|
| [DiSpel Cockpit](https://github.com/Cambio-Project/dispel-cockpit)   | The Cockpit provides a visual user interface and coordinates the other tools. It allows to store and manage scenarios and analysis results. |
| [PSP Wizard](https://github.com/Cambio-Project/PSPWizardExtended)   | The PSPWizard allows for the machine-assisted creation of Property Specification Patterns (PSPs), which serve as stimuli and responses in scenarios. |
| [MiSim](https://github.com/Cambio-Project/MiSim)   | MiSim simulates a microservice system with customizable capacities, loadbalancing strategies, network delays and other real-world (resilience) factors. Stimuli in the form of PSP can be interpreted by MiSim. |
| [MoSIM](https://github.com/Cambio-Project/MoSIM)   | MoSIM searches in monitoring data for occurrences of stimuli specified as PSPs. |
| [TBVerifier](https://github.com/Cambio-Project/transient-behavior-verifier)    | The TBVerifiers enables verifying the scenario satisfaction on collected system data through use of te underlying MTL solvers.
| [TQPropRefiner](https://github.com/Cambio-Project/transient-behavior-requirement-refiner)   | The TQPropRefiner is a tool for the refinement of temporal components and metric parameters of a PSP. |

The following tools are currently not integrated into the DiSpel process:

| **Component** | **Short Description** |
|---------------|-----------------------|
| [RESIRO](https://github.com/Cambio-Project/hazard-elicitation)   |  RESIRIO is a chatbot approach for helping developers to create resilience scenarios. |
| [TransVis frontend](https://github.com/Cambio-Project/conversational-transient-behavior-visualization-backend/tree/master) & [TransVis backend](https://github.com/Cambio-Project/conversational-transient-behavior-visualization-frontend/tree/master)  | TransVis visualizes the transient behavior (i.e. QoS over time) of a microservice system. Additionally offers a chatbot for interactive analysis. |
| [SAE Tool](https://github.com/Cambio-Project/software-architecture-extraction)   |  The SAE tool uses event traces of a microservice application to create an architectural model for MiSim. |

The following libraries are no standalone tools but used as part of other DiSpel toling.

| **Component** | **Short Description** |
|---------------|-----------------------|
| [TL-Tea](https://github.com/Cambio-Project/TL-Tea)   | TL-Tea parses and converts LTL and MTL formulas into tree structures and can act as a LTL/MTL solver that analyzers like MiSim and MoSIM interact with. |


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

