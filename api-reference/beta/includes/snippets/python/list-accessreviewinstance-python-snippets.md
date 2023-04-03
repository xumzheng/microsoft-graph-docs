---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = InstancesRequestBuilderGetRequestConfiguration();

queryParameters = InstancesRequestBuilderGetQueryParameters();
queryParameters.top = 100;
queryParameters.skip = 0;

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.identityGovernance().accessReviews().definitionsById('accessReviewScheduleDefinition-id').instances().get(requestConfiguration);


```