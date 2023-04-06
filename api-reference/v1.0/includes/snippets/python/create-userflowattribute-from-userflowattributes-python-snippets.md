---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IdentityUserFlowAttribute()
request_body.setDisplayName('Hobby')

request_body.setDescription('Your hobby')

request_body.setDataType(IdentityUserFlowAttributeDataType('string'))


request_config = UserFlowAttributesRequestBuilderPostRequestConfiguration(
request_config = UserFlowAttributesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.identity.userFlowAttributes.post(request_body, headers=)


```