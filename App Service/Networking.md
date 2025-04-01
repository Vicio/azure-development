App service provides a series of features to control network traffic:
* Inbound traffic control
	* Restrictions based on IP or IP ranges
* Outbound traffic control
	* Restrictions based on IP or IP ranges
	* VNet integration
* Private endpoints
	* Allows app services to be available only through internal network
	* Only available for Premium plan or higher
* Hybrid connections
	* Allows connections to on-premises servers
	* Requires the Hybrid Connection Manager installed on the on-premises servers
* DNS & custom domains
	* DNS private resolution
	* Allows mapping of domains purchased with another vendor
* Network security groups integration
	* Allows the usage of grouping and tagging to restrict access via the Azure Firewall
* Dedicated network environment
	* Allows deploying your own vNet to isolate your app services
	* Dedicated IPs
	* Supports load balancing
	* Only available in Isolated tier