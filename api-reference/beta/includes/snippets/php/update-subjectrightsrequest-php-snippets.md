---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SubjectRightsRequest();


$requestRequestBody->setInternalDueDateTime(new DateTime("2021-08-30T00:00:00Z"));
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.subjectRightsRequest',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->privacy()->subjectRightsRequestsById('subjectRightsRequest-id')->patch($requestRequestBody);


```