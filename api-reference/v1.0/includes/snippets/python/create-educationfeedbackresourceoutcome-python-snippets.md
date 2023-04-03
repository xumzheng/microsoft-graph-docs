---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationOutcome();
requestBody.set@odatatype('#microsoft.graph.educationFeedbackResourceOutcome');

additionalData = [
'feedbackResource' => requestBody = FeedbackResource();
		requestBody.set@odatatype('#microsoft.graph.educationWordResource');

		requestBody.setDisplayName('Document1.docx');


requestBody.setFeedbackResource($feedbackResource);

];
requestBody.setAdditionalData(additionalData);




result = awaitclient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').outcomes().post(requestBody);


```