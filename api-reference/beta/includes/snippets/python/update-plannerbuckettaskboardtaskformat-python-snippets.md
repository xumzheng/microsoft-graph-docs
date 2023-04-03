---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PlannerBucketTaskBoardTaskFormat();
requestBody.setOrderHint('A6673H Ejkl!');


request_config = BucketTaskBoardFormatRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

request_config.headers = headers;


result = awaitclient.planner().tasksById('plannerTask-id').bucketTaskBoardFormat().patch(requestBody, request_config);


```