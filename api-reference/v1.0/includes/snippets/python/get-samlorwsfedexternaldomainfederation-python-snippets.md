---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = IdentityProviderBaseRequestBuilderGetRequestConfiguration();

queryParameters = IdentityProviderBaseRequestBuilderGetQueryParameters();
queryParameters.filter = "domains/any";

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.directory().federationConfigurationsById('identityProviderBase-id').get(requestConfiguration);


```