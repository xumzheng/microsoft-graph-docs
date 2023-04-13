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

created_by = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.created_by = createdBy



result = await client.security.triggerTypes.retentionEventTypes.post(request_body = request_body)


```