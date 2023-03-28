---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new Oauth2PermissionGrantsRequestBuilderGetRequestConfiguration();

$queryParameters = new Oauth2PermissionGrantsRequestBuilderGetQueryParameters();
$queryParameters->filter = "clientId eq 'b0d9b9e3-0ecf-4bfd-8dab-9273dd055a94' and principalId eq '3fbd929d-8c56-4462-851e-0eb9a7b3a2a5' and consentType eq 'Principal'";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->oauth2PermissionGrants()->get($requestConfiguration);


```