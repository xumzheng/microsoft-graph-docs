---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerBucketTaskBoardTaskFormat()
request_body.setOrderHint('A6673H Ejkl!')


request_config = BucketTaskBoardFormatRequestBuilderPatchRequestConfiguration(
request_config = BucketTaskBoardFormatRequestBuilderPatchRequestConfiguration(query_params=)
headers['Prefer'] = "return=representation"
headers['If-Match'] = "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""


result = await client.planner.tasks_by_id('plannerTask-id').bucketTaskBoardFormat.patch(request_body, request_config, headers=request_config)


```