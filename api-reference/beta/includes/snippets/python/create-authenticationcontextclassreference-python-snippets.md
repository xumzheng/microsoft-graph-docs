---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthenticationContextClassReference()
request_body.setId('c1')

request_body.setDisplayName('Contoso medium')

request_body.setDescription('Medium protection level defined for Contoso policy')

request_body.setIsAvailable(true)


request_config = AuthenticationContextClassReferencesRequestBuilderPostRequestConfiguration(
request_config = AuthenticationContextClassReferencesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identity.conditionalAccess.authenticationContextClassReferences.post(request_body, headers=)


```