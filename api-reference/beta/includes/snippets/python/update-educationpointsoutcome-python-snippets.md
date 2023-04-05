---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationOutcome()
request_body.set@odatatype('#microsoft.graph.educationPointsOutcome')

additionalData = [
'points' => request_body = Points()
		request_body.set@odatatype('#microsoft.graph.educationAssignmentPointsGrade')

		request_body.setPoints(85.0)


request_body.setPoints($points)

];
request_body.setAdditionalData(additionalData)




result = await client.education.classesby_id('educationClass-id').assignmentsby_id('educationAssignment-id').submissionsby_id('educationSubmission-id').outcomesby_id('educationOutcome-id').patch(request_body)


```