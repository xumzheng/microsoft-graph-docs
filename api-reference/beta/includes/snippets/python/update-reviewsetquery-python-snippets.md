---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReviewSetQuery()
request_body.setDisplayName('My Query 1 - Renamed')



result = await client.compliance.ediscovery.cases_by_id('case-id').reviewSets_by_id('reviewSet-id').queries_by_id('reviewSetQuery-id').patch(request_body, headers=)


```