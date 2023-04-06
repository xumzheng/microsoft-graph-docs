---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Tag()
request_body.setDescription('This is an updated description.')



result = await client.compliance.ediscovery.cases_by_id('case-id').tags_by_id('tag-id').patch(request_body, headers=)


```