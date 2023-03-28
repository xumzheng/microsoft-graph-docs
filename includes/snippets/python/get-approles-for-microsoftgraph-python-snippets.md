---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ServicePrincipalsRequestBuilderGetRequestConfiguration();

$queryParameters = new ServicePrincipalsRequestBuilderGetQueryParameters();
$queryParameters.filter = "displayName eq 'Microsoft Graph'";
$queryParameters.select = ["id","displayName","appId","appRoles"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.servicePrincipals().get($requestConfiguration);


```