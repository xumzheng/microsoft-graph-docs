---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Tag()
request_body.setDescription('This is an updated description.')



result = await client.compliance_ediscovery_casesby_id('case-id')_tagsby_id('tag-id').patch(request_body)


```