---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReviewSetQuery()
request_body.setDisplayName('My Query 1')

request_body.setQuery('(subject:\"Quarterly Financials\")')



result = await client.compliance.ediscovery.cases._by_id('case-id').reviewSets._by_id('reviewSet-id').queries.post(request_body)


```