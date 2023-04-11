---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlowAttribute()
request_body.displayName = 'Hobby'

request_body.description = 'Your hobby'

request_body.DataType(IdentityUserFlowAttributeDataType('string'))



request_configuration = UserFlowAttributesRequestBuilderPostRequestConfiguration(
)


result = await client.identity.userFlowAttributes.post(request_body = request_body)


```