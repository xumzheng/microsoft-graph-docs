---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2xIdentityUserFlow()
request_body.setId('Partner')

request_body.setUserFlowType(UserFlowType('signuporsignin'))

request_body.setUserFlowTypeVersion(1)

identityProvidersIdentityProvider1 = IdentityProvider()
identityProvidersIdentityProvider1.setId('Facebook-OAuth')

identityProvidersIdentityProvider1.setType('Facebook')

identityProvidersIdentityProvider1.setName('Facebook')


identityProvidersArray []= identityProvidersIdentityProvider1;
request_body.setIdentityProviders(identityProvidersArray)




result = await client.identity.b2xUserFlows.post(request_body)


```