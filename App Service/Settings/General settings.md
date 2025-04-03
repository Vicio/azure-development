In the general settings there are two major sections, the stack settings and the platform settings.

#### Stack settings
In the stack settings you can configure the software stack to be used for your web application, it can be either a predefined stack from azure, or a custom one using a container image.

The predefined stacks available as of now are:
* .NET
	* .NET Core
	* .NET Framework
	* ASP.NET
* Java
* Node.JS
* Python
* PHP
* Ruby
* Go
#### Platform settings
In the platform settings you can configure what the host is going to have and how it is going to behave, the settings available are these:
* Bitness: either 32 or 64 bit application, exclusive for windows.
* FTP: enable or disable FTP for file upload
* HTTP version
* Web sockets
* Always On: Tells the app service to keep the application loaded. It does so by constantly pinging the app.
* ARR affinity: Ties the session of a user to an instance, only applicable when there is more than one app instance.
* HTTPS only
* Minimum TLS version
* Debugging: allow temporary remote debugging, it disables itself after 48 hours of enabling it.