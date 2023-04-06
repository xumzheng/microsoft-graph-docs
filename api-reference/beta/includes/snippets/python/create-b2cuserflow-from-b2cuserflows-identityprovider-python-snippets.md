---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2cIdentityUserFlow()
request_body.setId('Customer')

request_body.setUserFlowType(UserFlowType('signuporsignin'))

request_body.setUserFlowTypeVersion(3)

identityProvidersIdentityProvider1 = IdentityProvider()
identityProvidersIdentityProvider1.setId('Facebook-OAuth')


identityProvidersArray []= identityProvidersIdentityProvider1;
request_body.setIdentityProviders(identityProvidersArray)



request_config = B2cUserFlowsRequestBuilderPostRequestConfiguration(
request_config = B2cUserFlowsRequestBuilderPostRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.identity.b2cUserFlows.post(request_body, request_config, headers=request_config)


```