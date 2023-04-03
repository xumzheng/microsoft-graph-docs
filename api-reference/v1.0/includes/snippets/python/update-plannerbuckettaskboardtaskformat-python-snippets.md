---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PlannerBucketTaskBoardTaskFormat();
requestBody.setOrderHint('A6673H Ejkl!');


requestConfiguration = BucketTaskBoardFormatRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.planner().tasksById('plannerTask-id').bucketTaskBoardFormat().patch(requestBody, requestConfiguration);


```