---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

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
recurrence = PlannerTaskRecurrence();
recurrenceSchedule = PlannerRecurrenceSchedule();
recurrenceSchedulePattern = RecurrencePattern();
recurrenceSchedulePattern.setType(RecurrencePatternType('daily'));

recurrenceSchedulePattern.setInterval(3);


recurrenceSchedule.setPattern($recurrenceSchedulePattern);
recurrenceSchedule.setPatternStartDateTime(DateTime('2022-02-22T02:10:33Z'));


recurrence.setSchedule($recurrenceSchedule);

requestBody.setRecurrence($recurrence);

requestConfiguration = PlannerTaskRequestBuilderPatchRequestConfiguration();

headers = [
	'Prefer' => 'return=representation',
	'If-Match' => 'W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="',
];

requestConfiguration.headers = headers;


requestResult = graphServiceClient.planner().tasksById('plannerTask-id').patch(requestBody, requestConfiguration);


```