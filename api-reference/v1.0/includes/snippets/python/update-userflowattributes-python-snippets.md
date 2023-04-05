---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlowAttribute()
request_body.setDescription('Your new hobby')



result = await client.identity_userFlowAttributesby_id('identityUserFlowAttribute-id').patch(request_body)


```