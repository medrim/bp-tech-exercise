####
Hello World Python App using Azure Pipeline and Azure Function

| Requirements    | Task          | Current Status | Finished | 
|-----------------|---------------|----------------|----------|
|Create a simple 'Hello World' Python app (can be Dockerised) that will be run as an Azure Function | Simple Python App | Awaiting Review |
|During the build phase run one example of code testing or scanning | Setup and configure SonarQube server | Awaiting Review | 
|Demonstrate both pass and fail scenarios in the build history if possible| | Awaiting Review |
|Create a release pipeline that deploys your Python app as an Azure Function| Setup a Azure function resource and task to deploy | Awaiting Review | 
|This should be a multi-stage (multi-environment) release pipeline with stages that reflect a realistic route-to-live Each environment’s release stage can be very simple and need only perform an Azure Function deployment The pipeline should also, however, aim to demonstrate relevant examples in some, or all, of the following areas. | Multi stage deployments | Awaiting Review | 
|Use of pre- and post-deployment conditions| Add pre- and post-deployment conditions | Awaiting Review | 
|Your deployed Azure function should result in a response from a testable endpoint| See Endpoints below| Awaiting Review |

**Azure DevOps project can be found here**  
https://dev.azure.com/medrim/bp-tech-exercise

**Main pipeline can be found here for multi-stage deployments**  
 https://dev.azure.com/medrim/bp-tech-exercise/_releaseProgress?_a=release-pipeline-progress&releaseId=12

**Testable endpoints**

| Environment Name | Endpoints |
|------------------|----------|
| DEV | https://bp-tech-dev.azurewebsites.net/api/HelloWorld?name=World
| TEST | https://bp-tech-test.azurewebsites.net/api/HelloWorld?name=World
| QA | https://bp-tech-qa.azurewebsites.net/api/HelloWorld?name=World
| PROD | https://bp-tech-prod.azurewebsites.net/api/HelloWorld?name=World

**SonarQube Analysis report**  
https://bptechtestdns.azurewebsites.net/dashboard?id=BP-Sonarqube-Tech-Test
