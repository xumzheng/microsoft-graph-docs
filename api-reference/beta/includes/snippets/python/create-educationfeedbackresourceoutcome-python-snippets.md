---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationOutcome()
request_body.@odatatype = '#microsoft.graph.educationFeedbackResourceOutcome'

additionalData = [
'feedbackResource' => request_body = FeedbackResource()
		request_body.@odatatype = '#microsoft.graph.educationWordResource'

		request_body.displayName = 'Document1.docx'


request_body.feedbackResource = feedbackResource

];
request_body.additionaldata(additionalData)




request_configuration = OutcomesRequestBuilderPostRequestConfiguration(
)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').outcomes.post(request_body = request_body)


```