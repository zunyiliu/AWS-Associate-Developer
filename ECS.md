Amazon Elastic Container Service (Amazon ECS) is a fully managed container orchestration service that helps you easily deploy, manage, and scale containerized applications
## Task Definitin
A task definition is a blueprint for your application. It is a text file in JSON format that describes the parameters and one or more containers that form your application.
## Task placement strategy
A task placement strategy is an algorithm for selecting instances for task placement or tasks for termination. 
### binpack 
Tasks are placed on container instances so as to leave the least amount of unused CPU or memory. This strategy minimizes the number of container instances in use. 
### random 
Tasks are placed randomly. 
### spread 
Tasks are placed evenly based on the specified value.
## launch types
1. EC2 launch type -- large workloads that must be price optimized.  
2. Fargate launch type -- no need for provisioning and managing the underlying infrastructure.  
## port mapping
containerPort is the port that the container exposes.  
hostPort is the port you want to map it to on the host.Set 0 and it will dynamically assign available port to you  
