The Azure services offer both automated and manual deployment.

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
