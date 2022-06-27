---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReview();


$requestRequestBody->setDisplayName('TestReview new name');
$result =  $graphClient->accessReviewsById('accessReview-id')->patch($requestRequestBody);


```