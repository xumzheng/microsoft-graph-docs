---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestConfiguration = new SourceCollectionRequestBuilderGetRequestConfiguration();

$queryParameters = new SourceCollectionRequestBuilderGetQueryParameters();
$queryParameters->expand = ["addToReviewSetOperation","custodianSources","lastEstimateStatisticsOperation"];

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->compliance()->ediscovery()->casesById('case-id')->sourceCollectionsById('sourceCollection-id')->get($requestConfiguration);


```