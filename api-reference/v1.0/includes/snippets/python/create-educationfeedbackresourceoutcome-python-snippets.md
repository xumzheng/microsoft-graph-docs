---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationOutcome()
request_body.set@odatatype('#microsoft.graph.educationFeedbackResourceOutcome')

additionalData = [
'feedbackResource' => request_body = FeedbackResource()
		request_body.set@odatatype('#microsoft.graph.educationWordResource')

		request_body.setDisplayName('Document1.docx')


request_body.setFeedbackResource($feedbackResource)

];
request_body.setAdditionalData(additionalData)




result = await client.education_classesby_id('educationClass-id')_assignmentsby_id('educationAssignment-id')_submissionsby_id('educationSubmission-id')_outcomes.post(request_body)


```