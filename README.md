This repository houses code for a simple .NET application as well as a deployment pipeline to restore, test and build the project. It also creates a container image, uploads it to Azure Container Registry, and publishes the new revision of the application to Azure Container Apps across Dev/Prod environments. 

Each environment should contain the following secrets:

- ACR_PASSWORD - Token which is used by github runners to upload container image to Azure Container Registry. 

Each environment should contain the following environment variables:

- ACR_NAME - Name of the Azure Container Registry for the given environment.
- ACR_USERNAME - Username associated with the ACR token (see secret above).
- AZURE_CLIENT_ID - App ID of Service Principal used by deployment.
- AZURE_SUBSCRIPTION_ID - ID of subscription where the container app is being deployed.
- AZURE_TENANT_ID - ID of Entra tenant where Service Principal exists.
- RESOURCE_GROUP - Name of resource group where Azure infrastructure is being deployed.

| Language | Framework | Platform | Author |
| -------- | -------- |--------|--------|
| ASP.NET Core | .NET Core 2.2 | Azure Web App, Virtual Machines |

# ASP.NET Core MVC application

Sample ASP.NET Core MVC application.

## License:

See [License](#)

## Contributing

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/). For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

