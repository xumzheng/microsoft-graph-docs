---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = ServicePrincipalsRequestBuilderGetRequestConfiguration();

queryParameters = ServicePrincipalsRequestBuilderGetQueryParameters();
queryParameters.filter = "displayName eq 'Microsoft Graph'";
queryParameters.select = ["id","displayName","appId","oauth2PermissionScopes"];

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.servicePrincipals().get(requestConfiguration);


```