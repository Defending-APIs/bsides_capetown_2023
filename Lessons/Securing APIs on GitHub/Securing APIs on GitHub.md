# Authorization
In this lesson, you will learn to secure yur APIs with GitHub Actions by constructing a pipeline that will scan your OpenAPI specification for vulnerabilities and test the API implementation for compliance with the specification.

## Setup
All that is required to run this lesson is to fork the 42Crunch sample pipeline from [here](https://github.com/42Crunch/apisecurity-tutorial). You will also need to explicitly enable GitHub Actions in your forked repository.

## Instructions

### Step 1: Run the 42Crunch API Security Audit
Manually trigger the execution of the 42Crunch API Security Audit by clicking on the `Actions` tab in your forked repository and then clicking on the `42Crunch API Security Audit` workflow. Click on the `Run workflow` button to start the workflow. Use the `Security` tab to find the `Code scanning` results and examine the findings.

### Step 2: Run the 42Crunch API  Security Scan
Manually trigger the execution of the 42Crunch API Security Scan by clicking on the `Actions` tab in your forked repository and then clicking on the `42Crunch API Security Scan` workflow. Click on the `Run workflow` button to start the workflow. Use the Security tab to find the Code scanning results and examine the findings.

### Step 3: Add these two workflows to your pull-request workflow
Use GitHub settings to protect your main branch, and then create a pull request to merge changes to the `PhotoManager.json` file in the repository. Verify that both the audit and the scan are running in your pull request workflow. Understand the behavior of how GitHub manages pull requests with open security issues. Try remediating some of the issues or deliberately introducing new issues to see how GitHub handles them.

## Further Reading
* [42Crunch sample GitHub pipeline](https://github.com/42Crunch/apisecurity-tutorial)
* [GitHub Actions documentation](https://docs.github.com/en/actions)
