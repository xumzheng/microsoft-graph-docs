---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Group();


$requestRequestBody->setDescription('Group assignable to a role');
$requestRequestBody->setDisplayName('Role assignable group');
$requestRequestBody->setGroupTypes( [
'Unified',],
$requestRequestBody->setIsAssignableToRole(True);
$requestRequestBody->setMailEnabled(True);
$requestRequestBody->setSecurityEnabled(True);
$requestRequestBody->setMailNickname('contosohelpdeskadministrators');
$requestRequestBodyAdditionalData = [
	"owners@odata.bind" =>  [
'https://graph.microsoft.com/v1.0/users/99e44b05-c10b-4e95-a523-e2732bbaba1e',	],
	"members@odata.bind" =>  [
'https://graph.microsoft.com/v1.0/users/6ea91a8d-e32e-41a1-b7bd-d2d185eed0e0','https://graph.microsoft.com/v1.0/users/4562bcc8-c436-4f95-b7c0-4f8ce89dca5e',	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->groups()->post($requestRequestBody);


```