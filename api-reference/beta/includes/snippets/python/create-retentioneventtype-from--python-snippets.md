---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RetentionEventType()
request_body.set@odatatype('#microsoft.graph.security.retentionEventType')

request_body.setDisplayName('String')

request_body.setDescription('String')

createdBy = IdentitySet()
createdBy.set@odatatype('microsoft.graph.identitySet')


request_body.setCreatedBy($createdBy)

request_config = RetentionEventTypesRequestBuilderPostRequestConfiguration(
request_config = RetentionEventTypesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.security.triggerTypes.retentionEventTypes.post(request_body, headers=)


```