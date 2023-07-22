Amazon Elastic Container Service (Amazon ECS) is a fully managed container orchestration service that helps you easily deploy, manage, and scale containerized applications
## Task
A task definition is a blueprint for your application. It is a text file in JSON format that describes the parameters and one or more containers that form your application.
## Task placement strategy
A task placement strategy is an algorithm for selecting instances for task placement or tasks for termination. 
### binpack 
Tasks are placed on container instances so as to leave the least amount of unused CPU or memory. This strategy minimizes the number of container instances in use. 
### random 
Tasks are placed randomly. 
### spread 
Tasks are placed evenly based on the specified value.
