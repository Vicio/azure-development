App service provides built-in authentication support, which enables developers to enable security features into their app without adding more code. The built-in authentication works by creating a new container that has the authentication application which receives all network traffic before handing it to the application.

There are some limitations for this built-in feature, the first one is that it cannot interact directly with the application, meaning there is no room for customization. The other one is that it is limited to specific providers:
* Microsoft Entra
* Facebook
* Google
* X
* GitHub
* OpenID compliant providers