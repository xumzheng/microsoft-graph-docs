---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new DecisionsRequestBuilderGetRequestConfiguration();

$queryParameters = new DecisionsRequestBuilderGetQueryParameters();
$queryParameters->top = 100;
$queryParameters->skip = 0;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->me()->pendingAccessReviewInstancesById('accessReviewInstance-id')->decisions()->get($requestConfiguration);


```