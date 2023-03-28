---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new ServicePrincipalRequestBuilderGetRequestConfiguration();

$queryParameters = new ServicePrincipalRequestBuilderGetQueryParameters();
$queryParameters.select = ["customSecurityAttributes"];

$requestConfiguration.queryParameters = $queryParameters;


$requestResult = $graphServiceClient.servicePrincipalsById('servicePrincipal-id').get($requestConfiguration);


```