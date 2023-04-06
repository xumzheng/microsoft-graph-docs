---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_configuration = SourceCollectionRequestBuilderGetRequestConfiguration(
request_configuration = SourceCollectionRequestBuilderGetRequestConfiguration(query_params=query_params = SourceCollectionRequestBuilderGetQueryParameters()
query_params['expand'] = ["addToReviewSetOperation","custodianSources","lastEstimateStatisticsOperation"]

)
query_params = SourceCollectionRequestBuilderGetQueryParameters()
query_params['expand'] = ["addToReviewSetOperation","custodianSources","lastEstimateStatisticsOperation"]

)


result = await client.compliance.ediscovery.cases_by_id('case-id').sourceCollections_by_id('sourceCollection-id').get(request_configuration)


```