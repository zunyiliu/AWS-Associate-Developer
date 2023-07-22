CodeDeploy is a deployment service that automates application deployments to Amazon EC2 instances, on-premises instances, serverless Lambda functions, or Amazon ECS services. 
## AppSpec
The AppSpec file is used to manage each deployment as a series of lifecycle event hooks, which are defined in the file.
### AppSpec hooks sections
ECS deployment-- BeforeInstall -> AfterInstall -> AfterAllowTestTraffic -> BeforeAllowTraffic -> AfterAllowTraffic 
Lambda deployment -- BeforeAllowTraffic  -> AfterAllowTraffic
