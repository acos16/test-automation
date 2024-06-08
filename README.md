# Test Automation

In this project you will find information to help you get started with test automation, understand its benefits, and provide sample frameworks and CI pipeline setups.

## Table of Contents
1. [Introduction](#introduction)
2. [What is Test Automation?](#what-is-test-automation)
3. [Benefits of Test Automation](#benefits-of-test-automation)
4. [Practice Sites](#practice-sites)
5. [Sample Frameworks](#sample-frameworks)
    - [Selenide](#selenide)
    - [Playwright](#playwright)
6. [API Automation](#api-automation)
7. [CI Pipelines](#ci-pipelines)
    - [Jenkins](#jenkins)
    - [GitHub Actions](#github-actions)
8. [Code Review Practices](#code-review-practices)


## Introduction
Automation is crucial in today’s industry, but starting can be sometimes daunting. This project aims to simplify the journey.

## What is Test Automation?
Test automation involves using software tools to run repeatable tests on your application, ensuring quality and efficiency. More details about what is test automation in [understanding-test-automation](01-test-automation.md).

## Benefits of Test Automation
What does automation bring to the table and what to automate can be found [here](02-benefits-test-automation.md).

## Practice Sites
- Practice Automation - List of [sites](03-practice-automation-sites.md) to use in your learning path.

## Sample Frameworks

### Selenide
A [sample framework](https://github.com/acos16/selenide-java-test-automation-framework) using Selenide for browser automation.


### Playwright
A sample framework using Playwright for modern web testing. --> TBA

## API Automation
Guides and samples for API automation. --> TBA

## CI Pipelines

### Jenkins
A [sample Jenkinsfile]() defining a Jenkins pipeline for building, testing and deploying a project.

#### Details about the pipeline
- Setting up a CI pipeline with Jenkins:
  - Place the Jenkinsfile in the root directory 
  - Jenkins pipeline includes steps for checking out code, compiling, running tests, publishing test results
- Several other steps can be added: code scanner, check code style/code formatted, etc.
- To add the Jenkinsfile to Jenkins server as pipeline job, follow steps described [here](https://www.btc-embedded.com/how-to-set-up-jenkins-from-scratch-on-your-own-pc-in-5-minutes/)

### GitHub Actions
A [sample yaml file](08-ci-qa-pipeline.yaml) using GitHub actions.

#### Details about the pipeline
- Setting up GitHub Actions for CI/CD:
  - Place the workflow file in `.github/workflows`. 
  - Workflow  can be run manually because it uses `workflow_dispatch`. Use the “Run workflow” feature in the Actions tab.
  - It is presumed that the execution of tests is done through a gradle task
  - It is applicable for a Java project
- To enhance this CI pipeline several other steps can be added: code scanner, check code style/code formatted, etc. 
  - There are plenty of plugins that can be used in this scope:
    - Code scanner: SonarQube, CodeQl 
    - Code style: Spotless, Checkstyle
- Further documentation on [GitHub actions](https://docs.github.com/en/actions/quickstart)
- A concrete implementation of a workflow is available in [this repository](https://github.com/acos16/selenide-java-test-automation-framework/tree/main).


## Code Review Practices