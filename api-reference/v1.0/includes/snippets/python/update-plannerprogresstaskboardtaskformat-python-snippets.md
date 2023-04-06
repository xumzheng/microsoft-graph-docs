---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerProgressTaskBoardTaskFormat()
request_body.setOrderHint('A6673H Ejkl!')


request_config = ProgressTaskBoardFormatRequestBuilderPatchRequestConfiguration(
request_config = ProgressTaskBoardFormatRequestBuilderPatchRequestConfiguration(query_params=)
headers['Prefer'] = "return=representation"
headers['If-Match'] = "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""


result = await client.planner.tasks_by_id('plannerTask-id').progressTaskBoardFormat.patch(request_body, request_config, headers=request_config)


```