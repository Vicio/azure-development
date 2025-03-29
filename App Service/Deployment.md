The Azure services offer both automated and manual deployment. ^5fa4b1

For automated deployment they offer three options:
* Azure DevOps Services: An option to upload, build and publish your app altogether in a single service.
* GitHub: Azure makes use of GitHub actions to build and process the deployment of an application.
* BitBucket: Works similar to GitHub.

For manual deployment they offer four options:
* Git: You can connect any git compliant repository to Azure to deploy the application.
* CLI: ```az webapp up``` command packages your app for deployment
* Zip deploy: You can manually upload a zipped file to the app service
* FTP/FTPS: Azure also allows to directly push your files with FTP like traditional hosting sites.
## Deployment slots
This is a feature that enables copies of your application, but pointing to a different version of it, such as a staging or development version. Allowing you to test the new changes included in those branches. 

There is also the possibility to have a percentage of the production traffic to move to these deployment slots in order to have users test the new changes firsthand and help with bug catching.

Once one of the slots can be considered mature enough, it can be swapped with the production slot to include the new changes without having any downtime in your app.

## Sidecar containers
These are used to deploy extra features to your already existing app, and that can be auxiliary services, such as monitoring, logging, configuration, and networking.