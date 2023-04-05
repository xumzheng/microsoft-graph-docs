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


result = await client.education_classesby_id('educationClass-id')_assignmentsby_id('educationAssignment-id')_submissionsby_id('educationSubmission-id')_outcomes.get(request_config)


```