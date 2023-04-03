---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = AccessReviewsRequestBuilderGetRequestConfiguration();

query_params = AccessReviewsRequestBuilderGetQueryParameters();
query_params.filter = "businessFlowTemplateId eq '6e4f3d20-c5c3-407f-9695-8460952bcc68'";
query_params.top = 100;
query_params.skip = 0;

request_config.queryParameters = query_params;


result = await client.accessReviews().get(request_config);


```