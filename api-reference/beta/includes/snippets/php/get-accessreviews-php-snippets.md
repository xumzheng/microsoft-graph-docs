---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestConfiguration = new AccessReviewsRequestBuilderGetRequestConfiguration();

$queryParameters = new AccessReviewsRequestBuilderGetQueryParameters();
$queryParameters->filter = 'businessFlowTemplateId%20eq%20\'6e4f3d20-c5c3-407f-9695-8460952bcc68\'';
$queryParameters->top = 100;
$queryParameters->skip = 0;

$requestConfiguration->queryParameters = $queryParameters;


$result =  $graphClient->accessReviews()->get($requestConfiguration);


```