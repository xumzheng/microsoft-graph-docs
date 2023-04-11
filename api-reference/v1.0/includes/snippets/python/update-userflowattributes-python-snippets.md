---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlowAttribute()
request_body.description = 'Your new hobby'



request_configuration = IdentityUserFlowAttributeRequestBuilderPatchRequestConfiguration(
)


result = await client.identity.userFlowAttributes_by_id('identityUserFlowAttribute-id').patch(request_body = request_body)


```