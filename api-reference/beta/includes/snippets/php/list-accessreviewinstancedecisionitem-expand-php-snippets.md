---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AccessReviewInstanceDecisionItemRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessReviewInstanceDecisionItemRequestBuilderGetQueryParameters();
$queryParameters->expand = 'instance($expand=definition)';

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->identityGovernance()->accessReviews()->decisionsById('accessReviewInstanceDecisionItem-id')->get($requestConfiguration);


```