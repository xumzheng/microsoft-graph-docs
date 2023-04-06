---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RecommendationsRequestBuilderGetRequestConfiguration(
request_configuration = RecommendationsRequestBuilderGetRequestConfiguration(query_params=query_params = RecommendationsRequestBuilderGetQueryParameters()
query_params['filter'] = "recommendationType eq 'turnOffPerUserMFA'"

)
query_params = RecommendationsRequestBuilderGetQueryParameters()
query_params['filter'] = "recommendationType eq 'turnOffPerUserMFA'"

)


result = await client.directory.recommendations.get(request_configuration)


```