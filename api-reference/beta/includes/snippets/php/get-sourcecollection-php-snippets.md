---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new SourceCollectionRequestBuilderGetRequestConfiguration();

$queryParameters = new SourceCollectionRequestBuilderGetQueryParameters();
$queryParameters->expand = 'addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->sourceCollectionsById('sourceCollection-id')->get($requestConfiguration);


```