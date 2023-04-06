---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkPosition()
request_body.setIsCurrent(true)


request_config = WorkPositionRequestBuilderPatchRequestConfiguration(
request_config = WorkPositionRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.profile.positions_by_id('workPosition-id').patch(request_body, headers=)


```