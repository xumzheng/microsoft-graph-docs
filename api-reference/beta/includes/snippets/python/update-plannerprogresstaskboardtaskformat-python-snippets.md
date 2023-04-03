---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PlannerProgressTaskBoardTaskFormat();
requestBody.setOrderHint('A6673H Ejkl!');


request_config = ProgressTaskBoardFormatRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

request_config.headers = headers;


result = await client.planner().tasksById('plannerTask-id').progressTaskBoardFormat().patch(requestBody, request_config);


```