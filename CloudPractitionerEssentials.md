<!-- TOC -->
- [Definitions](#definitions)
- [Purchase Options](#purchase-options)
- [Scaling Options](#scaling-options)
  - [Auto Scaling](#auto-scaling)
    - [Auto Scaling group](#auto-scaling-group)
<!-- /TOC -->


## Definitions
| Term                          | Definition                                                                 |
|-------------------------------|----------------------------------------------------------------------------|
| AWS (Amazon Web Services)     | A comprehensive and evolving cloud computing platform provided by Amazon. |
| Cloud Computing               | The on-demand delivery of IT resources over the Internet with pay-as-you-go pricing. |
| Region                        | A geographical area containing multiple AWS Availability Zones.           |
| Availability Zone (AZ)        | One or more discrete data centers with redundant power and networking.    |
| Edge Location                 | A site that AWS uses to cache content closer to users, used in services like CloudFront. |
| IAM (Identity and Access Management) | A service for managing access to AWS services and resources securely.  |
| EC2 (Elastic Compute Cloud)   | A web service that provides resizable compute capacity in the cloud.       |
| S3 (Simple Storage Service)   | An object storage service that offers scalability, data availability, and security. |
| RDS (Relational Database Service) | A managed relational database service supporting multiple database engines. |
| Lambda                        | A serverless compute service that runs code in response to events.        |
| CloudFormation                | A service for modeling and setting up AWS resources using templates.      |
| Auto Scaling                  | A service that automatically adjusts compute capacity to maintain performance. |
| Elastic Load Balancing (ELB)  | A service that automatically distributes incoming application traffic.    |
| AWS Global Infrastructure     | The physical components (Regions, AZs, Edge Locations) of AWS.            |
| CloudFront                    | A fast content delivery network (CDN) service.                            |
| AWS Trusted Advisor           | A tool that provides real-time guidance to help provision resources.      |
| AWS Well-Architected Framework | A set of best practices to help build secure, high-performing, resilient, and efficient infrastructure. |
| Pricing Calculator            | A tool for estimating the cost of AWS services.                          |
| Support Plans                 | Tiered support offerings for AWS customers (Basic, Developer, Business, Enterprise). |
| Shared Responsibility Model   | A model defining AWS and customer responsibilities in the cloud.          |
| Hypervisor                    | Software that creates and runs virtual machines by abstracting hardware resources. |
| Tenant                        | A single customer or user group using a shared computing resource.         |
| Multitenancy                  | An architecture where multiple tenants share the same physical resources while maintaining data isolation. |


## Purchase Options
| Plan                          | Definition                                                                 |
|-------------------------------|----------------------------------------------------------------------------|
| On Demand     | Pay per hour/sec, this can provide you with a baseline. no longterm commitment |
| Savings Plan    | Low prices with hourly spend commitment for 1 or 3 year term (save 72%) |
| Standard Reserved Instance | Steady state workloads. This option is a good fit if you know the EC2 instance type and size you need for your steady-state applications and in which AWS Region you plan to run them. 3 payment options(full, partial, no upfront cost), (save up to 75%) |
| Convertable Reserved Instance | Steady state workloads. If you need to run your EC2 instances in different Availability Zones or different instance types. 3 payment options(full, partial, no upfront cost), (save up to 75%) |
| Spot Instances | AWS provide 2min warning before reclamation (save up to 90%) |
| Dedicated hosts | Physical servers with Amazon EC2 instance capacity that is fully dedicated to your use. (Most expensive) |


## Scaling Options
Scalability involves beginning with only the resources you need and designing your architecture to automatically respond to changing demand by scaling out or in. As a result, you pay for only the resources you use. You don’t have to worry about a lack of computing capacity to meet your customers’ needs.
| Plan                          | Definition                                                                 |
|-------------------------------|----------------------------------------------------------------------------|
| Dynamic scaling    | Responds to changing demand. |
| Predictive scaling    | Automatically schedules the right number of Amazon EC2 instances based on predicted demand. |

### Auto Scaling
In the cloud, computing power is a programmatic resource, so you can take a more flexible approach to the issue of scaling. By adding Amazon EC2 Auto Scaling to an application, you can add new instances to the application when necessary and terminate them when no longer needed.

#### Auto Scaling group
When you create an Auto Scaling group, you can set the minimum number of Amazon EC2 instances. The minimum capacity is the number of Amazon EC2 instances that launch immediately after you have created the Auto Scaling group. In this example, the Auto Scaling group has a minimum capacity of one Amazon EC2 instance. You pay for only the instances you use, when you use them.
![Autoscaling Group](Autoscaling.png)

