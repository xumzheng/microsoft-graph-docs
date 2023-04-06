---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OutcomesRequestBuilderGetRequestConfiguration(
request_config = OutcomesRequestBuilderGetRequestConfiguration(query_params=params['filter'] = "isof('microsoft.graph.educationFeedbackResourceOutcome')"
)


result = await client.education.classes_by_id('educationClass-id').assignments_by_id('educationAssignment-id').submissions_by_id('educationSubmission-id').outcomes.get(request_config, headers=request_config)


```