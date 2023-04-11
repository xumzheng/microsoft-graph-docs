---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReviewSetQuery()
request_body.displayName = 'My Query 1'

request_body.query = '(subject:\"Quarterly Financials\")'



request_configuration = QueriesRequestBuilderPostRequestConfiguration(
)


result = await client.compliance.ediscovery.cases_by_id('case-id').reviewSets_by_id('reviewSet-id').queries.post(request_body = request_body)


```