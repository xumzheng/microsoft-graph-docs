---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationOutcome();
requestBody.set@odatatype('#microsoft.graph.educationPointsOutcome');

additionalData = [
'points' => requestBody = Points();
		requestBody.set@odatatype('#microsoft.graph.educationAssignmentPointsGrade');

		requestBody.setPoints(85.0);


requestBody.setPoints($points);

];
requestBody.setAdditionalData(additionalData);




result = awaitclient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').outcomesById('educationOutcome-id').patch(requestBody);


```