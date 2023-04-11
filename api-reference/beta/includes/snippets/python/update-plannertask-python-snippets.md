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
		assignments.@odatatype = '#microsoft.graph.plannerAssignment'

		assignments.orderHint = 'N9917 U2883!'


assignments.fbab97d049324511b675204639209557 = fbab97d0-4932-4511-b675-204639209557

];
assignments.additionaldata(additionalData)



request_body.assignments = assignments
appliedCategories = PlannerAppliedCategories()
additionalData = [
'category3' => true,
'category4' => false,
];
appliedCategories.additionaldata(additionalData)



request_body.appliedCategories = appliedCategories
recurrence = PlannerTaskRecurrence()
recurrenceSchedule = PlannerRecurrenceSchedule()
recurrenceSchedulePattern = RecurrencePattern()
recurrenceSchedulePattern.Type(RecurrencePatternType('daily'))

recurrenceSchedulePattern.interval = 3


recurrenceSchedule.pattern = recurrenceSchedulePattern
recurrenceSchedule.patternStartDateTime = DateTime('2022-02-22T02:10:33Z')


recurrence.schedule = recurrenceSchedule

request_body.recurrence = recurrence


request_configuration = PlannerTaskRequestBuilderPatchRequestConfiguration(
headers = {
					'Prefer' : "return=representation",
					'If-Match' : "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc=\"",
}

)


result = await client.planner.tasks_by_id('plannerTask-id').patch(request_body = request_body, request_configuration = request_configuration)


```