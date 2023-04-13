---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2xIdentityUserFlow()
request_body.id = 'Partner'

request_body.UserFlowType(UserFlowType('signuporsignin'))

request_body.user_flow_type_version = 1

identity_providers_identity_provider1 = IdentityProvider()
identityProvidersIdentityProvider1.id = 'Facebook-OAuth'

identityProvidersIdentityProvider1.type = 'Facebook'

identityProvidersIdentityProvider1.name = 'Facebook'


identityProvidersArray []= identityProvidersIdentityProvider1;
request_body.identityproviders(identityProvidersArray)





result = await client.identity.b2xUserFlows.post(request_body = request_body)


```