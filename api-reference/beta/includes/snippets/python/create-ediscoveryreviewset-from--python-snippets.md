---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryReviewSet()
request_body.setDisplayName('My review set 2')



result = await client.security_cases_ediscoveryCasesby_id('ediscoveryCase-id')_reviewSets.post(request_body)


```