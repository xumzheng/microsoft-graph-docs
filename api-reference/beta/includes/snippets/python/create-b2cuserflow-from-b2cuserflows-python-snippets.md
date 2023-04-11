---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2cIdentityUserFlow()
request_body.id = 'Customer'

request_body.UserFlowType(UserFlowType('signuporsignin'))

request_body.userFlowTypeVersion = 3



request_configuration = B2cUserFlowsRequestBuilderPostRequestConfiguration(
)


result = await client.identity.b2cUserFlows.post(request_body = request_body)


```