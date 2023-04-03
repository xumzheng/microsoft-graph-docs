---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

request_config = InstancesRequestBuilderGetRequestConfiguration();

query_params = InstancesRequestBuilderGetQueryParameters();
query_params.top = 100;
query_params.skip = 0;

request_config.queryParameters = query_params;


result = awaitclient.identityGovernance().accessReviews().definitionsById('accessReviewScheduleDefinition-id').instances().get(request_config);


```