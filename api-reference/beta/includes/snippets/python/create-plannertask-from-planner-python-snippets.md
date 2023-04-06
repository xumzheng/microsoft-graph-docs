---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerTask()
request_body.setPlanId('xqQg5FS2LkCp935s-FIFm2QAFkHM')

request_body.setBucketId('hsOf2dhOJkqyYYZEtdzDe2QAIUCR')

request_body.setTitle('Update client list')

assignments = PlannerAssignments()
additionalData = [
'fbab97d0-4932-4511-b675-204639209557' => assignments = Fbab97d0-4932-4511-b675-204639209557()
		assignments.set@odatatype('#microsoft.graph.plannerAssignment')

		assignments.setOrderHint(' !')


assignments.setFbab97d0-4932-4511-b675-204639209557($fbab97d0-4932-4511-b675-204639209557)

];
assignments.setAdditionalData(additionalData)



request_body.setAssignments($assignments)

request_config = TasksRequestBuilderPostRequestConfiguration(
request_config = TasksRequestBuilderPostRequestConfiguration(query_params=)


result = await client.planner.tasks.post(request_body, headers=)


```