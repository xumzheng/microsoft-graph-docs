---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = PlannerTaskRequestBuilderDeleteRequestConfiguration();

headers = [
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

request_config.headers = headers;


awaitclient.planner().tasksById('plannerTask-id').delete(request_config);


```