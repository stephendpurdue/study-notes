
#### Load Balancing:

Load balancing can be used to effectively distribute date to other EC2 instances that are in low use, this is an effective method of traffic distribution. ELB can manage both inbound and outbound traffic.

There are several routing methods that can be used in ELB, they include:

- Round Robin: Offers even, cyclic distribution of data.
- Least Connections: Routes packets to the server with the least load.
- IP Hashing: Stores the IP of a user to ensure they land on the same server.
- Least Response Time: Routes packets to the server with the fastest response time.

#### Messaging & Queuing:

Information can be stored in a buffer to reduce load.
Applications can talk to each other to share information, this is referred to as a tightly-coupled architecture.

Example:

A -> B, B -> A

If server A fails, server B will jump in to take the load, and vice-versa.

SQS (Simple Queue Service): stores information in a queue to ensure effective load balancing, or if a server goes offline.

SNS (Simple Notification Service: A service that allows messages or notifications to be sent to end-users.

#### EventBridge:

This is a serverless service that bridges / connects between different parts of an application or AWS setup. This can be used to simplify the process of sending / receiving data on AWS.


#### AWS Lambda: 

This is a serverless compute service that can be used to trigger events on applications, these are called lambda functions. It follows a simple workflow:

Upload code -> Set triggers -> Run code when triggered -> Pay only for compute used.

#### Containers (Docker in the cloud):

Similar to docker, this service allows for program information to be stored in containers, fixing the classic issue of 'it works on my machine but not yours', this packages all the information such as dependencies, configs, and code, into one container, that can be distributed in the cloud.

Example of container services:

ECS:  Allows for containers to be run in the cloud.

EKS: Kubernetes service to manage more complex container deployments.

ECR: Registry of containers, stores container images.

Containers can be deployed to either EC2 or Fargate.