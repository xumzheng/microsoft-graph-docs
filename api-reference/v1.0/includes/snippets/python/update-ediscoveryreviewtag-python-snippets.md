---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryReviewTag()
request_body.displayName = 'My tag API 2'

request_body.description = 'Use Graph API to create tags (updated)'




result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').tags_by_id('ediscoveryReviewTag-id').patch(request_body = request_body)


```