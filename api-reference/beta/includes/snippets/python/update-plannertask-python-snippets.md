---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerTask()
assignments = PlannerAssignments()
additionalData = [
'fbab97d0-4932-4511-b675-204639209557' => assignments = Fbab97d0-4932-4511-b675-204639209557()
		assignments.set@odatatype('#microsoft.graph.plannerAssignment')

		assignments.setOrderHint('N9917 U2883!')


assignments.setFbab97d0-4932-4511-b675-204639209557($fbab97d0-4932-4511-b675-204639209557)

];
assignments.setAdditionalData(additionalData)



request_body.setAssignments($assignments)
appliedCategories = PlannerAppliedCategories()
additionalData = [
'category3' => true,
'category4' => false,
];
appliedCategories.setAdditionalData(additionalData)



request_body.setAppliedCategories($appliedCategories)
recurrence = PlannerTaskRecurrence()
recurrenceSchedule = PlannerRecurrenceSchedule()
recurrenceSchedulePattern = RecurrencePattern()
recurrenceSchedulePattern.setType(RecurrencePatternType('daily'))

recurrenceSchedulePattern.setInterval(3)


recurrenceSchedule.setPattern($recurrenceSchedulePattern)
recurrenceSchedule.setPatternStartDateTime(DateTime('2022-02-22T02:10:33Z'))


recurrence.setSchedule($recurrenceSchedule)

request_body.setRecurrence($recurrence)

request_config = PlannerTaskRequestBuilderPatchRequestConfiguration()

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
]

request_config.headers = headers


result = await client.planner.tasks._by_id('plannerTask-id').patch(request_body, request_config)


```