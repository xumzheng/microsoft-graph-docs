---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryReviewTag()
request_body.setDisplayName('My tag API 2')

request_body.setDescription('Use Graph API to create tags (updated)')



result = await client.security.cases.ediscoveryCasesby_id('ediscoveryCase-id').tagsby_id('ediscoveryReviewTag-id').patch(request_body)


```