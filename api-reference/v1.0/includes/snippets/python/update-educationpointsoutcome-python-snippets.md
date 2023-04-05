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




result = await client.education_classesby_id('educationClass-id')_assignmentsby_id('educationAssignment-id')_submissionsby_id('educationSubmission-id')_outcomesby_id('educationOutcome-id').patch(request_body)


```