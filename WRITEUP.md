# Write-up Template



# Virtual Machine vs Web App Service
Azure Virtual Machines (VMs) provide infrastructure as a service (IaaS) by allowing you to create and use virtual machines in the cloud. While, Azure App Service is an HTTP-based service for hosting web applications, REST APIs, and mobile back ends. It is a Platform as a Service (PaaS) that allows a developer to focus on the application while Azure takes care of the infrastructure.

Each of these services has its own strenght and appropriate use cases. Virtual Machines are ususally a better choice when user want to control the underlying operating system or using customized software; without these needs of system and software control and high-performance demand on computing, an app service is typically a better choice due to its lightweight.

# Why do I choose Web App in this project?
Azure Web App is functional enough to provide platform, web API and mobile backends. It has a well designed built-in associated services for security, mantainence and so on. It is also very flexsible on scalability to support the demand. Compared with Virtual Machine, it is more likely to promise quick built-up and deployment. while for virtual machine, I need more effort on system maintainenece.

# Analyze, choose, and justify the appropriate resource option for deploying the app
- cost: Since Web App Service is lightweighted, especially compared with Virtual Machine, it is very possible it is more unexpensive under same computing tasks. It has Free and Shared plans for small tasks. Besides these, it has built-in load balancers to adjust structure for saving cost.

- Scalability: Web App Serivce has very flexsible capability on scaling. The amount of vCPUs or RAM, remote storage, pricing tier are all included in choices. It also has auto scaling options.

- Availability: Web App Serices has high availability accross a large scale of global regions. It has SLA which is the sum of all Deployment Minutes across all Apps deployed by Customer in a given Azure subscription, promising high availability.

- Workflow: Azure App service support multiple deployment approaches, like GitHub, Azure DevOps, or any Git repository. This provides convenience for developers.

# Assess app changes that would change your decision

- Web App serivce has limitation on hardware and scale. If there is a large amount grow in users and the ariticle's size, then Virtual Machine is more adorable since it can be scaled up easily both through its computing volume and the number of VMs. It is also possible to have better control of hardware and operation system to get all functions more efficient.

- If there is need to create more advanced functions and traffic manangement in future, virtual machine is always a better choice since developer can have authority on system and software design and development.

- If there is need to use language which is not supported by Web App in future, then we have to choose VM for deployment. 

- If there is need to have contorl on operation system, then it is indeed to move to VM.