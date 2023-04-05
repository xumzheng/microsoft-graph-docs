---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LegalHold()
request_body.set@odatatype('#microsoft.graph.ediscovery.legalHold')

request_body.setDescription('String')

createdBy = IdentitySet()
createdBy.set@odatatype('microsoft.graph.identitySet')


request_body.setCreatedBy($createdBy)
request_body.setIsEnabled(boolean)

request_body.setStatus(LegalHoldStatus('string'))

request_body.setContentQuery('String')

request_body.setErrors(['String', ])

request_body.setDisplayName('String')



result = await client.compliance.ediscovery.casesby_id('case-id').legalHolds.post(request_body)


```