# test-automation

As we look at the industry's evolution, automation has become a necessary skill. But starting with automation can be sometimes daunting.

In this project, I'd like to go through:

1. [What is test automation](01-test-automation.md)
2. [Benefits of test automation](02-benefits-test-automation.md)
3. [Sites to practice automation](03-practice-automation-sites.md)
4. [Test automation sample framework with selenide](https://github.com/acos16/selenide-java-test-automation-framework)
5. Test automation sample framework with playwright
6. API automation
7. CI pipeline with Jenkins
8. [CI pipeline with GitHub actions](07-ci-qa-pipeline.yaml)

```
To set up GitHub Actions for running Gradle tests, you need to create a workflow file in your repository. 
This file should be located in the .github/workflows directory of your repository and place the yaml file there.


To manually trigger a GitHub Actions workflow, you can use the “Run workflow” feature on the Actions tab of your GitHub repository. Here’s how to do it:

	1.	Go to your GitHub repository.
	2.	Click on the “Actions” tab at the top.
	3.	In the left sidebar, you’ll see a list of workflows. Click on the workflow you want to run manually (in this case, it’s likely named “CI Pipeline”).
	4.	In the upper-right corner, you’ll see a green button labeled “Run workflow”. Click on it.
	5.	You’ll be prompted to select the branch for which you want to run the workflow. Choose the branch (usually main or master) and click the “Run workflow” button.

Once you’ve done this, GitHub will start running the workflow on the selected branch. You can monitor the progress and view the results in real-time on the Actions tab.


Additionally, other steps can be added to the pipeline.

Add code scanners, such as SonarQube

- name: SonarQube Scan
  uses: SonarSource/sonarcloud-github-action@master
  env:
  GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
  SONAR_TOKEN: ${{ secrets.SONAR_TOKEN }}

Make sure you have a SonarQube server set up and the necessary tokens (GITHUB_TOKEN and SONAR_TOKEN) added as secrets in your GitHub repository settings.

Alternative to SonarQube: CodeQl
```

An implementation of a GitHub action workflow is available in [this repository](https://github.com/acos16/selenide-java-test-automation-framework/tree/main)


9. Practices for Code review



