---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PlannerAssignedToTaskBoardTaskFormat();
orderHintsByAssignee = PlannerOrderHintsByAssignee();
additionalData = [
'aaa27244-1db4-476a-a5cb-004607466324' => '8566473P 957764Jk!', 
];
orderHintsByAssignee.setAdditionalData(additionalData);



requestBody.setOrderHintsByAssignee($orderHintsByAssignee);

requestConfiguration = AssignedToTaskBoardFormatRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.planner().tasksById('plannerTask-id').assignedToTaskBoardFormat().patch(requestBody, requestConfiguration);


```