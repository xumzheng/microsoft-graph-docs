---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ContinuousAccessEvaluationPolicy();


$requestRequestBody->setMigrate(True);
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.continuousAccessEvaluationPolicy',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identity()->continuousAccessEvaluationPolicy()->patch($requestRequestBody);


```