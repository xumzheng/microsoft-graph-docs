---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = InstancesRequestBuilderGetRequestConfiguration(
request_configuration = InstancesRequestBuilderGetRequestConfiguration(query_params=query_params = InstancesRequestBuilderGetQueryParameters()
query_params['top'] = 100
query_params['skip'] = 0

)
query_params = InstancesRequestBuilderGetQueryParameters()
query_params['top'] = 100
query_params['skip'] = 0

)


result = await client.identityGovernance.accessReviews.definitions_by_id('accessReviewScheduleDefinition-id').instances.get(request_configuration)


```