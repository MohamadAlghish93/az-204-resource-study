# az-204-resource-study
Resource help in study azure 204 developer  


Azure role-based access control (Azure RBAC) 


Lock down inbound traffic to your Azure Virtual Machines with Microsoft Defender for Cloud's just-in-time (JIT) virtual machine (VM) access feature.

Deploment Slots

Cosmos DB
	- Account
	- Database
	- Containers (Partion Key)
		- Document
		- Document
	- Consistency Levels

Storage blob
	- Sorage tiers

SAS (Shared Access Signauter)

---

VM
	- Availability zones
	- Availability sets
	- Load Balance
	(https://docs.microsoft.com/en-us/learn/modules/provision-virtual-machines-azure/3-azure-virtual-machine-availability-options)

---

Azure App Service Web Apps 
	- App Service plan
		- Shared compute: Both Free and Shared ( can't scale out. )
		- Dedicated compute: The Basic, Standard, Premium, PremiumV2, and PremiumV3
			(The higher the tier, the more VM instances are available to you for scale-out)
		- Isolated
			(It provides the maximum scale-out capabilities.)
		- Consumption
			(This tier is only available to function apps)

	- Outbound addresses

	- networking features of App Service can be used to control outbound network traffic
		( Hybrid Connections)

	- diagnostic logging
		- Application logging	
		- Web server logging	
		- Detailed error logging	
		- Failed request tracing	
		- Deployment logging	
		(https://docs.microsoft.com/en-us/learn/modules/configure-web-app-settings/5-enable-diagnostic-logging)

	- implement custom handlers 
		(https://docs.microsoft.com/en-us/learn/modules/serverless-go/7-knowledge-check)

---

Cosmos DB storage

	- Logical partitions
	- Physical partitions (10,000 RU/s,  50GB data)
	- correctly lists the two components of a partition key (Key path, key value)
	
	- consistency (https://docs.microsoft.com/en-us/learn/modules/use-consistency-models-azure-cosmos-db-sql-api/2-understand)
	
		
blob storage

	- Metadata (can be to container and sotrage account to be human readable)

	- (public access can be downloaded without any kind of authentication or auditing)
	
---

Implement user authentication and authorization

	- (https://docs.microsoft.com/en-us/learn/modules/explore-microsoft-identity-platform/3-app-service-principals)
		- application objects (how the service can issue tokens in order to access the application, resources that the application might need to access, and the actions that the application can take.)
		- service principals 
	
	- Permission types
		- Delegated permissions (with sign-in)
		- Application permissions (without sign-in)

	-  app scenarios require code to handle Conditional Access challenges
		(Apps performing the on-behalf-of flow)

	- With a multitenant app, you can't determine ahead of time which tenant will be used, so you need to use the 'https://login.microsoftonline.com/common' endpoint, which serves all Azure AD tenants.

	- security context for an application registered in Azure AD
		(service principal)

	- shared access signatures

		- User delegation SAS:  Azure Active Directory ( Blob storage only)
		- Service SAS: storage account key (Blob storage, Queue storage, Table storage, or Azure Files.)
		- Account SAS: storage account key (resources in one or more of the storage services. All of the operations available)

---

Monitor, troubleshoot, and optimize Azure solutions 

	- (https://docs.microsoft.com/en-us/learn/modules/develop-for-azure-cache-for-redis/2-azure-cache-redis-overview)

	- configure an app or service to use Application Insights

	- Linux, you need to use build-time instrumentation. Runtime instrumentation and automatic client-side telemetry are available only for Windows apps.


---

Connect to and consume Azure services and third-party services 

	- Implement API Management 

		- https://blog.cloudthat.com/12-sample-questions-to-help-you-crack-the-az-204-developing-microsoft-solutions-certification-exam/

	- Event Grid
		- Events - What happened.
		- Event sources - Where the event took place.
		- Topics - The endpoint where publishers send events. ( A topic is used for a collection of related events.)
			- System topics
			- Custom topics
		- Event subscriptions - The endpoint or built-in mechanism to route events, sometimes to more than one handler. Subscriptions are also used by handlers to intelligently filter incoming events.
		- Event handlers - The app or service reacting to the event. 

	- (https://docs.microsoft.com/en-us/learn/modules/implement-message-workflows-with-service-bus/2-choose-a-messaging-platform)


--- 

Blob storage tiers :
Premium, Hot, Cool and Archive




https://github.com/DishanRajapaksha/AZ-204
	

