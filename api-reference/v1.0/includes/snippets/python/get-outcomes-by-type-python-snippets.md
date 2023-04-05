---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_config = OutcomesRequestBuilderGetRequestConfiguration()

query_params = OutcomesRequestBuilderGetQueryParameters()
query_params.filter = "isof('microsoft.graph.educationFeedbackResourceOutcome')"

request_config.queryParameters = query_params


result = await client.education.classes._by_id('educationClass-id').assignments._by_id('educationAssignment-id').submissions._by_id('educationSubmission-id').outcomes.get(request_config)


```