---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryReviewSetQuery()
request_body.setDisplayName('My Query 1 (update)')

request_body.setContentQuery('(Author=\"edisons\")')



result = await client.security.cases.ediscoveryCasesby_id('ediscoveryCase-id').reviewSetsby_id('ediscoveryReviewSet-id').queriesby_id('ediscoveryReviewSetQuery-id').patch(request_body)


```