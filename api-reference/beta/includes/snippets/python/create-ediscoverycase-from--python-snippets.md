---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryCase()
request_body.displayName = 'CONTOSO LITIGATION-005'

request_body.description = 'Project Bazooka'

request_body.externalId = '324516'




result = await client.security.cases.ediscoveryCases.post(request_body = request_body)


```