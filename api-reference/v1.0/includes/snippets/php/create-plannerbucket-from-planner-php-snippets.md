---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerBucket();


$requestRequestBody->setName('Advertising');
$requestRequestBody->setPlanId('xqQg5FS2LkCp935s-FIFm2QAFkHM');
$requestRequestBody->setOrderHint(' !');
$result =  $graphClient->planner()->buckets()->post($requestRequestBody);


```