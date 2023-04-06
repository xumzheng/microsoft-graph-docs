---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Case()
request_body.setDisplayName('My Case 1 - Renamed')

request_body.setDescription('Updated description')

request_body.setExternalId('Updated externalId')



result = await client.compliance.ediscovery.cases_by_id('case-id').patch(request_body)


```