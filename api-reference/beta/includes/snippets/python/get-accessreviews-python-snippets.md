---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestConfiguration = AccessReviewsRequestBuilderGetRequestConfiguration();

queryParameters = AccessReviewsRequestBuilderGetQueryParameters();
queryParameters.filter = "businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'";
queryParameters.top = 100;
queryParameters.skip = 0;

requestConfiguration.queryParameters = queryParameters;


requestResult = graphServiceClient.accessReviews().get(requestConfiguration);


```