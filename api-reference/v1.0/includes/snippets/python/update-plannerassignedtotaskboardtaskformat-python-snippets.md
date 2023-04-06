---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerAssignedToTaskBoardTaskFormat()
orderHintsByAssignee = PlannerOrderHintsByAssignee()
additionalData = [
'aaa27244-1db4-476a-a5cb-004607466324' => '8566473P 957764Jk!', 
];
orderHintsByAssignee.setAdditionalData(additionalData)



request_body.setOrderHintsByAssignee($orderHintsByAssignee)

request_config = AssignedToTaskBoardFormatRequestBuilderPatchRequestConfiguration(
request_config = AssignedToTaskBoardFormatRequestBuilderPatchRequestConfiguration(query_params=)
headers['Prefer'] = "return=representation"
headers['If-Match'] = "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\""


result = await client.planner.tasks_by_id('plannerTask-id').assignedToTaskBoardFormat.patch(request_body, request_config, headers=request_config)


```