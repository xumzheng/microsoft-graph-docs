---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PlannerTask();
assignments = PlannerAssignments();
additionalData = [
'fbab97d0-4932-4511-b675-204639209557' => assignments = Fbab97d0-4932-4511-b675-204639209557();
		assignments.set@odatatype('#microsoft.graph.plannerAssignment');

		assignments.setOrderHint('N9917 U2883!');


assignments.setFbab97d0-4932-4511-b675-204639209557($fbab97d0-4932-4511-b675-204639209557);

];
assignments.setAdditionalData(additionalData);



requestBody.setAssignments($assignments);
appliedCategories = PlannerAppliedCategories();
additionalData = [
'category3' => true,
'category4' => false,
];
appliedCategories.setAdditionalData(additionalData);



requestBody.setAppliedCategories($appliedCategories);

request_config = PlannerTaskRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

request_config.headers = headers;


result = await client.planner().tasksById('plannerTask-id').patch(requestBody, request_config);


```