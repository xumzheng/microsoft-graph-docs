---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerTask()
request_body.planId = 'xqQg5FS2LkCp935s-FIFm2QAFkHM'

request_body.bucketId = 'hsOf2dhOJkqyYYZEtdzDe2QAIUCR'

request_body.title = 'Update client list'

assignments = PlannerAssignments()
additionalData = [
'fbab97d0-4932-4511-b675-204639209557' => assignments = Fbab97d0-4932-4511-b675-204639209557()
		assignments.@odatatype = '#microsoft.graph.plannerAssignment'

		assignments.orderHint = ' !'


assignments.fbab97d049324511b675204639209557 = fbab97d0-4932-4511-b675-204639209557

];
assignments.additionaldata(additionalData)



request_body.assignments = assignments


request_configuration = TasksRequestBuilderPostRequestConfiguration(
)


result = await client.planner.tasks.post(request_body = request_body)


```