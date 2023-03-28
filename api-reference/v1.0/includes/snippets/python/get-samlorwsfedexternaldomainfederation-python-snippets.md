---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new IdentityProviderBaseRequestBuilderGetRequestConfiguration();

$queryParameters = new IdentityProviderBaseRequestBuilderGetQueryParameters();
$queryParameters->filter = "domains/any";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->directory()->federationConfigurationsById('identityProviderBase-id')->get($requestConfiguration);


```