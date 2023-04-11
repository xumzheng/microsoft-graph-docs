---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerProgressTaskBoardTaskFormat()
request_body.orderHint = 'A6673H Ejkl!'


headers = {
		'Prefer' : "return=representation",
		'If-Match' : "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
}

)


result = await client.planner.tasks_by_id('plannerTask-id').progressTaskBoardFormat.patch(request_body = request_body, request_configuration = request_configuration)


```