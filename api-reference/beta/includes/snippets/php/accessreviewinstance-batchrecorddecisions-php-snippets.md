---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new BatchRecordDecisionsPostRequestBody();


$requestRequestBody->setDecision('Approve');
$requestRequestBody->setJustification('All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team');
$requestRequestBody->setResourceId('a5c51e59-3fcd-4a37-87a1-835c0c21488a');
$result =  $graphClient->me()->pendingAccessReviewInstancesById('accessReviewInstance-id')->batchRecordDecisions()->post($requestRequestBody);


```