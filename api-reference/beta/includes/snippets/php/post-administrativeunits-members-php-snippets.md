---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MembersPostRequestBody();


$requestRequestBodyAdditionalData = [
	"@odata.type" => '#Microsoft.Graph.Group',
	"description" => 'Self help community for golf',
	"displayName" => 'Golf Assist',
	"groupTypes" => ['Unified',],
"mailEnabled" => True,
"mailNickname" => 'golfassist',
"securityEnabled" => False,
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->administrativeUnitsById('administrativeUnit-id')->members()->post($requestRequestBody);


```