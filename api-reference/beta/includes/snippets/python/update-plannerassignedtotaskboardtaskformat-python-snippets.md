---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerAssignedToTaskBoardTaskFormat()
order_hints_by_assignee = PlannerOrderHintsByAssignee()
additionalData = [
'aaa27244-1db4-476a-a5cb-004607466324' => '8566473P 957764Jk!', 
];
orderHintsByAssignee.additionaldata(additionalData)



request_body.order_hints_by_assignee = orderHintsByAssignee


request_configuration = AssignedToTaskBoardFormatRequestBuilder.AssignedToTaskBoardFormatRequestBuilderPatchRequestConfiguration(
headers = {
		'Prefer' : "return=representation",
		'If-Match' : "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
}

)


result = await client.planner.tasks_by_id('plannerTask-id').assignedToTaskBoardFormat.patch(request_body = request_body, request_configuration = request_configuration)


```