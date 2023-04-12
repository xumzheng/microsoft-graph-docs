---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = OutcomesRequestBuilder.OutcomesRequestBuilderGetQueryParameters(
		filter = "isof('microsoft.graph.educationFeedbackResourceOutcome')",
)

request_configuration = OutcomesRequestBuilder.OutcomesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').outcomes.get(request_configuration = request_configuration)


```