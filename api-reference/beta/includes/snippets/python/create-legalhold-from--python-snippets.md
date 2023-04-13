---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LegalHold()
request_body.@odatatype = '#microsoft.graph.ediscovery.legalHold'

request_body.description = 'String'

created_by = IdentitySet()
createdBy.@odatatype = 'microsoft.graph.identitySet'


request_body.created_by = createdBy
request_body.is_enabled = Boolean

request_body.Status(LegalHoldStatus('string'))

request_body.contentQuery = 'String'

request_body.Errors(['String', ])

request_body.displayName = 'String'




result = await client.compliance.ediscovery.cases_by_id('case-id').legalHolds.post(request_body = request_body)


```