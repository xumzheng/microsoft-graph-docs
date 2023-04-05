---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryReviewSetQuery()
request_body.setDisplayName('My Query 1 (update)')

request_body.setContentQuery('(Author=\"edisons\")')



result = await client.security_cases_ediscoveryCasesby_id('ediscoveryCase-id')_reviewSetsby_id('ediscoveryReviewSet-id')_queriesby_id('ediscoveryReviewSetQuery-id').patch(request_body)


```