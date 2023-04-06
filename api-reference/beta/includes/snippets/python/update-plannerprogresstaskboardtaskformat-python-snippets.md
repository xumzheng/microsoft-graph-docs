---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerProgressTaskBoardTaskFormat()
request_body.setOrderHint('A6673H Ejkl!')


request_configuration = ProgressTaskBoardFormatRequestBuilderPatchRequestConfiguration(
request_configuration = ProgressTaskBoardFormatRequestBuilderPatchRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


result = await client.planner.tasks_by_id('plannerTask-id').progressTaskBoardFormat.patch(request_body, request_configuration)


```