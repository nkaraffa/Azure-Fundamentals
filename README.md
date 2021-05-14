# Azure-Fundamentals (AZ-900)
## What I learned about the Microsoft Azure platform
____________________________________________

	• Cloud computing is the delivery of computing services over the internet, enabling faster innovation, flexible resources, and economies of scale
		○ Compute, Networking, Storage, Analytics
		
	• Virtualization: the ability to create virtual machines (VM)
		○ Virtual machines have a Host server with OS, virtual hard-drive, and CPU
		
	• Azure cloud takes ownership of the Host server and rent out VMs
		○ Saves customer server space, utility costs, equipment cost, maintenance, etc.
		
	• Cloud Model 
		○ Public Cloud
			§ Owned by cloud service provider
			§ Provide resources and services to multiple organizations and users; accessed via secure internet connection
		○ Private Cloud
			§ Organization owned data center adds cloud server
			§ Organization does not share resources; fully responsible for services and maintenance
		○ Hybrid Cloud
			§ Most flexibility
			§ Organization determine where to run their applications; orgs control sercurity, compliance, or legal requirements
			
	• Cloud Benefits
		High availability	Fault tolerance	Scalability	Elasticity	Global Reach
		Customer Latency Capabilities	Agility	Predictive cost considerations	Disaster Recovery	Security
		
	• There are two different types of expenses that you should consider:
	
		• Capital Expenditure (CapEx) is the up-front spending of money on physical infrastructure, and then deducting that up-front expense over time. The up-front cost from CapEx has a value that reduces over time.
	
		• Operational Expenditure (OpEx) is spending money on services or products now, and being billed for them now. You can deduct this expense in the same year you spend it. There is no up-front cost, as you pay for a service or product as you use it.
		
	• Services (IaaS -> PaaS -> SaaS)
		• Infrastructure as a Service
			§ Build pay-as-you-go IT  infrastructure by renting servers, virtual machines, storage, networks, and OS from a cloud provider
		• Platform as a Service
			§ Provides environment for building, testing, and deploying software applications; without focusing on managing underlying infrastructure.
		• Software as a Service
			§ Users connect (i.e. Microsoft Teams)
			
	• Serverless Computing
		• With serverless computing application, the cloud service provider automatically provisions, scales, and manages the infrastructure 

Azure services
	• Region pairs - ensure data availability by having a backup datacenter around the world; at least 300 miles apart
	• Availability sets
		• Protects against outages; Physically separated datacenters within the same regions
	• Availability Zones
		• Protect against down-time from datacenter outages/failure; Physically separated datacenters within the same regions
	• Availability Options
		• tttt
	• Azure Resources
		• VM, Storage accounts, Virtual networks, App Services, SQL Databases, Functions
		
		• Resource group is a container to manage and aggregate resources in a single unit
			§ Can exist in different regions
			§ Only one resource type per group
			§ Assign permissions and use cases
			
		• Azure Resource Manager
			§ provides a management layer that enables you to create, update, and delete resources in your Azure subscriptions
			
	• Subscriptions
		• Billing boundary: generate separate billing reports and invoices for each subscription
		• Access control boundary: manage and control access to the resources that users can provision with specific subscriptions
		
	• Management Groups
		• Management groups include multiple Azure subscriptions

Azure Core Workloads
	• Azure compute services
		• Azure compute is an on-demand computing service that provides computing resources such as disks, processors, memory, networking, and OS
			§ VM, App services, Container Instances, Azure Kubernetes Services (AKS), Windows Virtual Desktop
		
Azure Networking Services
	• VNet & Subnets
		• Azure Virtual Networks (VNet) enables Azure resources to communicate with each other, the internet, and on-premises networks.
		• Subnets enable applications to run in the VNet
	• Virtual Private Network (VPN) Gateway
		• Used to send encrypted traffic between an Azure virtual network and an on-premises location over the public internet
	• Azure Express Route
		• Extends on-premises networks into Azure over a private connection that is facilitated by a connectivity provider
		
Azure Storage 
	• Container Storage (blob)
		• Optimized for storing massive amount of unstructured data, such as text or binary data
	• Disk Storage
		• Provides disks for virtual machines, applications, and other services to access and use
	• Azure Files
		• Highly available network file shares that can be accessed by using the standard Server Message Block (SMB) protocol
		
	• Azure storage access tiers
		• Hot
			§ Optimized for storing data that is accessed frequently
		• Cool
			§ Optimized for storing data that is infrequently accessed and stored for at least 30 days
		• Archive days 
			§ Optimized for storing data that is rarely accessed and stored for at least with flexible latency requirements

Management Tools
	• Azure Internet of Things (IoT) - IoT is the ability for devices to garner and then relay information for data analysis
		• Azure IoT Central = manage
			§ A fully managed global IoT SaaS solution that makes it easy to connect, monitor, and manage IoT assets at scale
		• Azure IoT Hub = message
		• Azure Sphere
	• Big data & analytics
		• Azure Synapse Analytics - cloud-based Enterprise data warehouse
		• Azure HDInsight - a fully-managed, open-source analytics service for enterprises
		• Azure Databricks - Apache Spark based analytics service
	• Artificial Intelligence & Machine Learning
		• Azure Machine Learning
		• Cognitive Services
		• Azure Bot Service
	• Azure Advisor
	• Azure Monitor
		• Log analytics, smart alerts, app insights, etc.
	• Azure 
	• Azure Resource Management (ARM)
		• Templates are JavaScript Object Notion (JSON) files that can be used to create and deploy Azure infrastructure without having to write programming objects.

Security (MODULE 4)
	• Azure Security Center
		• A monitoring service that provides threat protection across both Azure and on-premises datacenters
	• Azure Sentinel
		• A security information management (SEIM) and security automated response (SOAR) solution that provide security analytics and threat intelligence across an enterprise
	• Azure Key Vault
		• Stores application secrets in a centralized cloud location in order to securely control access permissions and access logging
	• Azure Dedicated Host
		• Provides physical servers that host one or more Azure virtual machines that is dedicated to a single organization's workload.


	• Defense in Depth
		• Layered approach to securing computer systems.
	• Network Security Groups (NSGs)
		• Filter network traffic to and from Azure resources on azure Virtual Networks.
	• Azure Firewall
		• A stateful, managed Firewall as a Service (FaaS) that grants/denies server access based on originating IP address, in order to protect network resources.
	• Azure Distributed Denial of Service (DDoS) protection
		• DDoS attacks overwhelm and exhaust network resources, making apps slow or unresponsive

Identity, governance, privacy, and compliance features (MODULE 5)
	• Terms:
		• Authentication: identifies the person or service seeking access to a resource
		• Authorization: determines an authenticated person's or service's level of access
		
	• Azure Active Directory (AAD) is Microsoft's Azure's cloud-based identity and access management service.
	• Tags:  places 'notes' on metadata
	• Azure Policy
		• Helps to enforce organizational standards and to assess compliance at-scale.
		• Provides governance and resource consistency with regulatory compliance, security, cost, and management.
	• Azure Blueprints
		• Makes it possible for development teams to rapidly build and stand up new environments.
		
	• Azure Trust Center:
		• Manages security, policy, and compliance

Azure Pricing and Lifecycle (MODULE 6)
	• Factors Affecting Costs:
		1. Resource Type
		2. Services
		3. Location
		4. Bandwidth
		5. Reserved Instances
		6. Azure Hybrid Use Benefit
		
