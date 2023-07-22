With Elastic Beanstalk, you can quickly deploy and manage applications in the AWS Cloud without having to learn about the infrastructure that runs those applications
### Create an application source bundle
When you use the AWS Elastic Beanstalk console to deploy a new application or an application version, you'll need to upload a source bundle. Your source bundle must meet the following requirements: 
1. Consist of a single ZIP file or WAR file (you can include multiple WAR files inside your ZIP file) 
2. Not exceed 500 MB 
3. Not include a parent folder or top-level directory (subdirectories are fine)
### Deployment policy
1. All at once – Deploy the new version to all instances simultaneously. All instances in your environment are out of service for a short time while the deployment occurs. 
2. Rolling – Deploy the new version in batches. Each batch is taken out of service during the deployment phase, reducing your environment's capacity by the number of instances in a batch. 
3. Rolling with additional batch – Deploy the new version in batches, but first launch a new batch of instances to ensure full capacity during the deployment process. 
4. Immutable – Deploy the new version to a fresh group of instances by performing an immutable update. 
5. Traffic splitting – Deploy the new version to a fresh group of instances and temporarily split incoming client traffic between the existing application version and the new one.
6. blue/green -- A blue/green deployment is a deployment strategy in which you create two separate, but identical environments. One environment (blue) is running the current application version and one environment (green) is running the new application version. 
