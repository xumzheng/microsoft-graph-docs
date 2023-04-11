---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationOutcome()
request_body.@odatatype = '#microsoft.graph.educationFeedbackOutcome'

additionalData = [
'feedback' => request_body = Feedback()
text = Text()
		text.content = 'This is feedback for the assignment as a whole.'

		text.contentType = 'text'


request_body.text = text

request_body.feedback = feedback

];
request_body.additionaldata(additionalData)




request_configuration = EducationOutcomeRequestBuilderPatchRequestConfiguration(
)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').outcomes_by_id('educationOutcome-id').patch(request_body = request_body)


```