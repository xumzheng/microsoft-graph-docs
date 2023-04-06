---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationOutcome()
request_body.set@odatatype('#microsoft.graph.educationFeedbackOutcome')

additionalData = [
'feedback' => request_body = Feedback()
text = Text()
		text.setContent('This is feedback for the assignment as a whole.')

		text.setContentType('text')


request_body.setText($text)

request_body.setFeedback($feedback)

];
request_body.setAdditionalData(additionalData)




result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').outcomes_by_id('educationOutcome-id').patch(request_body, headers=)


```