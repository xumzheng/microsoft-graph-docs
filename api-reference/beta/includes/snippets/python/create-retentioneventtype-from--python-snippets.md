---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = RetentionEventType()
request_body.@odatatype = '#microsoft.graph.security.retentionEventType'

request_body.displayName = 'String'

request_body.description = 'String'

createdBy = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.createdBy = createdBy


request_configuration = RetentionEventTypesRequestBuilderPostRequestConfiguration(
)


result = await client.security.triggerTypes.retentionEventTypes.post(request_body = request_body)


```