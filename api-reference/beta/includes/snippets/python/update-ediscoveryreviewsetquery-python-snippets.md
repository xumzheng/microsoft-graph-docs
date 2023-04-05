---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryReviewSetQuery()
request_body.setDisplayName('My Query 1 (update)')

request_body.setContentQuery('(Author=\"edisons\")')



result = await client.security.cases.ediscoveryCases._by_id('ediscoveryCase-id').reviewSets._by_id('ediscoveryReviewSet-id').queries._by_id('ediscoveryReviewSetQuery-id').patch(request_body)


```