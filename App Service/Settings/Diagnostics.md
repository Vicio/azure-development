App service web apps support built-in logging, the different types of logging are as follows:
* Windows only:
	* Web server logging: Any request data that is W3C compliant
	* Detailed HTTP error messages: HTML error debugging pages
	* Request failures tracing: A complete trace of all the components related to the issue and their interactions
* Any:
	* App logging: Logs thrown by the application itself
	* Deployment logging: Issues produced during web app creation, non-configurable

The supported storage for logging is the app service file system for all types and also storage blobs for app and web server logging.

For app logging a quota and retention days should be set before activating the service, and for web logging only retention days are required.

Logs can also be streamed to your local computer in real time using Azure CLI using the following command:
```bash
az webapp log tail --name appname --resource-group myResourceGroup
```

Log files can also be downloaded using the following URLs:
* Linux/containers: `https://<app-name>.scm.azurewebsites.net/api/logs/docker/zip`
* Windows: `https://<app-name>.scm.azurewebsites.net/api/dump`
