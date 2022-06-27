---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ActivateServicePlanPostRequestBody();


$requestRequestBody->setServicePlanId('28f42d6f-8034-4a0f-9d8a-a218a63b3299');
$requestRequestBody->setSkuId('465a2a90-5e59-456d-a7b8-127b9fb2e484');
$result =  $graphClient->me()->activateServicePlan()->post($requestRequestBody);


```