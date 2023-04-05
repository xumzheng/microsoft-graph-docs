---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryHoldPolicy()
request_body.setDescription('updated description')



result = await client.security.cases.ediscoveryCases._by_id('ediscoveryCase-id').legalHolds._by_id('ediscoveryHoldPolicy-id').patch(request_body)


```