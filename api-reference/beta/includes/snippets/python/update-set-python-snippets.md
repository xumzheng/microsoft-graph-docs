---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Set()
request_body.setDescription('mySet')


request_config = SetRequestBuilderPatchRequestConfiguration(
request_config = SetRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.termStore.sets_by_id('set-id').patch(request_body, headers=)


```