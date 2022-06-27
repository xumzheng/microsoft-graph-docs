---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewReviewer();


$requestRequestBody->setId('006111db-0810-4494-a6df-904d368bd81b');
$result =  $graphClient->accessReviewsById('accessReview-id')->reviewers()->post($requestRequestBody);


```