---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PlannerRosterMember();


$requestRequestBody->setUserId('String');
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.plannerRosterMember',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->planner()->rostersById('plannerRoster-id')->members()->post($requestRequestBody);


```