App service web apps support built-in logging, the different types of logging are as follows:
* Windows only:
	* Web server logging: Any request data that is W3C compliant
	* Detailed HTTP error messages: HTML error debugging pages
	* Request failures tracing: A complete trace of all the components related to the issue and their interactions
* Any:
	* App logging: Logs thrown by the application itself
	* Deployment logging: Issues produced during web app creation, non-configurable

The supported storage for logging is the app service file system for all types and also storage blobs for app and web server logging.

