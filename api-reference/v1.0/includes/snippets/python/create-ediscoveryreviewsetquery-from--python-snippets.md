---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryReviewSetQuery()
request_body.displayName = 'My Query 1'

request_body.contentQuery = '(Author=\"edison\")'



request_configuration = QueriesRequestBuilderPostRequestConfiguration(
)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').reviewSets_by_id('ediscoveryReviewSet-id').queries.post(request_body = request_body)


```