App service provides built-in authentication support, which enables developers to enable security features into their app without adding more code. The built-in authentication works by creating a new container that has the authentication application which receives all network traffic before handing it to the application.

There are some limitations for this built-in feature, the first one is that it cannot interact directly with the application, meaning there is no room for customization. The other one is that it is limited to specific providers:
* Microsoft Entra
* Facebook
* Google
* X
* GitHub
* OpenID compliant providers

### Authorization behavior
There are two behaviors that can be configured when a request from unknown user reaches the app:
* Allow unauthenticated requests: The App Service attaches a header to the user request that tells the application that the user is not authenticated, this allows the app to present a website for users that are not logged in.
* Require authentication: The App Service always redirects the user to a login page of the provider that has been specified for authentication.

### Token store
App Service also provides a built-in token store, which contains all tokens related with user authentication.
### Logging
If app logging is enabled, all traces related to authentication and authorization are logged.