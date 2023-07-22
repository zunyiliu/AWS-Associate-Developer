With Elastic Beanstalk, you can quickly deploy and manage applications in the AWS Cloud without having to learn about the infrastructure that runs those applications
## Create an application source bundle
When you use the AWS Elastic Beanstalk console to deploy a new application or an application version, you'll need to upload a source bundle. Your source bundle must meet the following requirements: 
1. Consist of a single ZIP file or WAR file (you can include multiple WAR files inside your ZIP file) 
2. Not exceed 500 MB 
3. Not include a parent folder or top-level directory (subdirectories are fine) 
