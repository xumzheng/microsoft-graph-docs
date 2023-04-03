---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = PendingAccessReviewInstancesRequestBuilderGetRequestConfiguration();

queryParameters = PendingAccessReviewInstancesRequestBuilderGetQueryParameters();
queryParameters.expand = ["definition"];
queryParameters.top = 100;
queryParameters.skip = 0;

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.me().pendingAccessReviewInstances().get(requestConfiguration);


```