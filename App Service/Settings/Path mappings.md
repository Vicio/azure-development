In this section you can configure how paths are going to be mapped in your web application. There are two options depending on the OS to be used as host for your app.

#### Windows
For Windows, all path configurations are done using IIS. With IIS you can configure how  some specific types of files should be treated, as well as defining the root directory of your web application, or multiple root directories for different apps.

#### Linux
In Linux you can make configurations only if you are using a container, and connect your app to a storage by creating a __New Azure Storage Mount__ with the following settings:
* Name
* Config options
* Storage acount
* Storage type
* Storage container
* Share name
* Access key
* Mount path
* Deployment slot (if slots are used)
