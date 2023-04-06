---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = RecommendationsRequestBuilderGetRequestConfiguration(
request_configuration = RecommendationsRequestBuilderGetRequestConfiguration(query_params=query_params = RecommendationsRequestBuilderGetQueryParameters()
query_params['filter'] = "id eq '0cb31920-84b9-471f-a6fb-468c1a847088_Microsoft.Identity.IAM.Insights.TurnOffPerUserMFA'"
query_params['expand'] = ["impactedResources"]

)
query_params = RecommendationsRequestBuilderGetQueryParameters()
query_params['filter'] = "id eq '0cb31920-84b9-471f-a6fb-468c1a847088_Microsoft.Identity.IAM.Insights.TurnOffPerUserMFA'"
query_params['expand'] = ["impactedResources"]

)


result = await client.directory.recommendations.get(request_configuration)


```