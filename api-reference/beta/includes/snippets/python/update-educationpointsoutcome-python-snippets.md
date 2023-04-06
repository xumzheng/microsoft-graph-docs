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



request_config = EducationOutcomeRequestBuilderPatchRequestConfiguration(
request_config = EducationOutcomeRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').outcomes_by_id('educationOutcome-id').patch(request_body, headers=)


```