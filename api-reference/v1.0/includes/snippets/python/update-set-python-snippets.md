---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Set()
request_body.description = 'mySet'



request_configuration = SetRequestBuilderPatchRequestConfiguration(
)


result = await client.sites_by_id('site-id').termStore.sets_by_id('set-id').patch(request_body = request_body)


```