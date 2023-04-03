---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EducationOutcome();
requestBody.set@odatatype('#microsoft.graph.educationFeedbackOutcome');

additionalData = [
'feedback' => requestBody = Feedback();
text = Text();
		text.setContent('This is feedback for the assignment as a whole.');

		text.setContentType('text');


requestBody.setText($text);

requestBody.setFeedback($feedback);

];
requestBody.setAdditionalData(additionalData);




result = awaitclient.education().classesById('educationClass-id').assignmentsById('educationAssignment-id').submissionsById('educationSubmission-id').outcomesById('educationOutcome-id').patch(requestBody);


```