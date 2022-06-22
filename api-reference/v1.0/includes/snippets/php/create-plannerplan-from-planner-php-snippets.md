---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerPlan();


$requestRequestBody->setOwner('ebf3b108-5234-4e22-b93d-656d7dae5874');
$requestRequestBody->setTitle('title-value');
$result =  $graphClient->planner()->plans()->post($requestRequestBody);


```