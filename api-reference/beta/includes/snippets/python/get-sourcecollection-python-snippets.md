---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_config = SourceCollectionRequestBuilderGetRequestConfiguration();

query_params = SourceCollectionRequestBuilderGetQueryParameters();
query_params.expand = ["addToReviewSetOperation","custodianSources","lastEstimateStatisticsOperation"];

request_config.queryParameters = query_params;


result = await client.compliance.ediscovery.casesById('case-id').sourceCollectionsById('sourceCollection-id').get(request_config);


```