CodeDeploy is a deployment service that automates application deployments to Amazon EC2 instances, on-premises instances, serverless Lambda functions, or Amazon ECS services. 
## AppSpec
The AppSpec file is used to manage each deployment as a series of lifecycle event hooks, which are defined in the file.
### AppSpec hooks sections
ECS deployment-- BeforeInstall -> AfterInstall -> AfterAllowTestTraffic -> BeforeAllowTraffic -> AfterAllowTraffic 
Lambda deployment -- BeforeAllowTraffic  -> AfterAllowTraffic

## deployment type
### In-place deployment
The application on each instance in the deployment group is stopped, the latest application revision is installed, and the new version of the application is started and validated. 
### Blue/green deployment
two seperate environments, blue for current green for new version, if green tests fine then switch to blue
