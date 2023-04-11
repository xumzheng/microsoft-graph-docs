---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

query_params = InstancesRequestBuilder.InstancesRequestBuilderGetQueryParameters(
				top = 100,
				skip = 0,
)

request_configuration = InstancesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)


result = await client.identityGovernance.accessReviews.definitions_by_id('accessReviewScheduleDefinition-id').instances.get(request_configuration = request_configuration)


```