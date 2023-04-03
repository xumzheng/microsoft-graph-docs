---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PlannerTask();
requestBody.setPlanId('xqQg5FS2LkCp935s-FIFm2QAFkHM');

requestBody.setBucketId('hsOf2dhOJkqyYYZEtdzDe2QAIUCR');

requestBody.setTitle('Update client list');

assignments = PlannerAssignments();
additionalData = [
'fbab97d0-4932-4511-b675-204639209557' => assignments = Fbab97d0-4932-4511-b675-204639209557();
		assignments.set@odatatype('#microsoft.graph.plannerAssignment');

		assignments.setOrderHint(' !');


assignments.setFbab97d0-4932-4511-b675-204639209557($fbab97d0-4932-4511-b675-204639209557);

];
assignments.setAdditionalData(additionalData);



requestBody.setAssignments($assignments);


result = await client.planner().tasks().post(requestBody);


```