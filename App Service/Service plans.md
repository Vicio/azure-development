A set of compute resources to run different [[App Service|app services]]. Each plan service defines:
* An OS
* A region (where data centers reside)
* A number of VMs
* The size of those VMs
* A Pricing tier:
	* Shared computing:
		* Free and shared tiers are here.
		* The hardware resources are shared among different users.
		* Cannot be scaled out.
	* Dedicated computing:
		* Basic, standard, and Premium v1, v2 and v3 tiers are here.
		* Dedicated hardware for the user.
		* Auto-scale option.
		* Multiple VMs available.
	* Isolated computing: ^6e5c1f
		* Isolated v1 and v2 tiers are here.
		* Dedicated hardware with dedicated network.
		* Auto-scale.
		* Maxed scale-out capabilities.
