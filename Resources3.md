
# What is orchestration?
Orchestration is the coordinated execution of multiple IT automation tasks or processes. Orchestration is usually applied across multiple computer systems, applications, and services to ensure that deployment, configuration management, and other processes are performed in the proper sequence. 

**Automation and orchestration are distinct**, but related concepts. 

**Automation** is the use of software to perform tasks without human intervention, to minimize errors and reduce the time spent manually performing the operations needed to deploy, manage, and scale IT applications and infrastructure. 

**Orchestration** coordinates automated tasks across multiple systems into higher-order workflows, so that individual tasks can work together to serve a specific function or process.

# Why is orchestration necessary?
IT teams manage a wide range of servers, systems, and applications across private datacenters, clouds, and edge locations. As IT environments become more complex, automating tasks can improve efficiency and make processes easier to manage—but scaling automation comes with its own challenges. 

Most IT processes involve many individual tasks that need to be automated. And to fully automate a process, the tasks that make it up also need to work together; when one task finishes, it needs to launch the appropriate follow-up task. Some automation solutions can connect tasks into logical workflows, removing the manual labor of triggering actions at the appropriate time. Building these workflows is one element of orchestration. 

But each part of a task can—on its own—involve multi-step workflows that depend on communicating with third-party systems. For example, provisioning a system would typically include orchestrating with hypervisors to create virtual machines, communicating with the network to ensure that connectivity is configured and established, and confirming that any required firewall policies have been put in place. This is where a comprehensive orchestration solution steps in; it can coordinate tasks across disparate systems, allowing IT teams to build fully automated workflows that span entire enterprise use cases.

# What does orchestration involve?
Depending on the use case, orchestration is often used to refer to some specific types of IT workflows and the tools that manage them. 

**Kubernetes** is a container orchestration tool; it is used to `automate the deployment` and `scaling of containerized applications`. 

**Jenkins** is used to orchestrate development pipelines; it executes workflows for `building`, `testing`, and `pushing code to a repository`. Both of these processes can be integrated into a larger automated workflow by a comprehensive orchestration solution that can coordinate tasks across third-party systems.

> Let’s look at a few example orchestration workflows for some common IT use cases. 

A `workflow` for **deploying a server** might include the following steps:

- Deploy the server.
- Configure the server.
- Assign storage capacity.
- Grab an application from a repository, install it, and configure it.  
- Talk to the firewall or load balancer to make sure it’s configured to allow this new system into its pool and policies.
- Update the company ITSM system to confirm that this server has been successfully deployed.
-----

# A workflow for provisioning a cloud instance might look like this:

- Provision the instance.
- Configure the operating system.
- Log a ticket in an ITSM system to inform it that the system is active.
- Update the firewall.
- Create necessary user accounts with appropriate permissions.
- Connect the system to an external database.



# What is Kubernetes?
Kubernetes is an open source container orchestration platform that automates the deployment, management, and scaling of containerized applications. It acts as an operating engine for cloud infrastructure, eliminating the manual steps required to configure and run applications or allocate resources.

A project of the Cloud Native Computing Foundation (CNCF), Kubernetes was first introduced in 2014 and has become a widely adopted platform for organizations to run distributed applications and services at scale.

# What are the basic concepts of Kubernetes?
The core concepts of Kubernetes center around clusters, nodes, and pods working together to run applications. A cluster represents the entire system, nodes are the individual machines doing the work, and pods are the smallest deployable units containing your application containers. 

The containers bundle the code, configuration, and dependencies of an application, allowing it to run as an isolated process with its own resources. Each application gets its own container or multiple containers, which are grouped into Kubernetes pods.

Kubernetes can run on bare metal servers, virtual machines, public cloud providers, private clouds, and hybrid cloud environments. One of Kubernetes’s key advantages is it works on many different kinds of infrastructure.

Kubernetes is built to help users to follow 3 core design principles, as explained in the Kubernetes implementation details. A Kubernetes deployment should be:

- Secure. It should follow the latest security best-practices.
- User-friendly. It should be operable using a few simple commands.
- Extendable. It shouldn’t favor one provider and should be customizable from a configuration file.

# What is a Kubernetes cluster?
A working Kubernetes deployment is called a cluster, which is a group of virtual or physical hosts that work together to run containerized applications.

# What is Knative and serverless Kubernetes?
Serverless Kubernetes is a cloud-native development model that lets developers run containerized applications without needing to manage clusters or pay for resources you don’t need. Knative is an open source extension that adds these native serverless capabilities to Kubernetes.

# What’s the difference between Kubernetes and Red Hat OpenShift?
The primary difference between Kubernetes and Red Hat OpenShift is that Kubernetes is an open source container orchestration engine, while Red Hat OpenShift is a complete, enterprise application platform built using Kubernetes as its foundation.





