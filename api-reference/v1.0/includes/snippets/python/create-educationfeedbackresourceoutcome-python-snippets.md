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



request_config = OutcomesRequestBuilderPostRequestConfiguration(
request_config = OutcomesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').outcomes.post(request_body, headers=)


```