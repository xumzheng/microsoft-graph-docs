---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryReviewSetQuery()
request_body.setDisplayName('My Query 1')

request_body.setContentQuery('(Author=\"edison\")')



result = await client.security_cases_ediscoveryCasesby_id('ediscoveryCase-id')_reviewSetsby_id('ediscoveryReviewSet-id')_queries.post(request_body)


```