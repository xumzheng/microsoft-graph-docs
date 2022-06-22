---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Group();


$requestRequestBody->setDescription('Group with designated owner and members');
$requestRequestBody->setDisplayName('Operations group');
$requestRequestBody->setGroupTypes( [
],
$requestRequestBody->setMailEnabled(False);
$requestRequestBody->setMailNickname('operations2019');
$requestRequestBody->setSecurityEnabled(True);
$requestRequestBodyAdditionalData = [
	"owners@odata.bind" =>  [
'https://graph.microsoft.com/beta/users/26be1845-4119-4801-a799-aea79d09f1a2',	],
	"members@odata.bind" =>  [
'https://graph.microsoft.com/beta/users/ff7cb387-6688-423c-8188-3da9532a73cc','https://graph.microsoft.com/beta/users/69456242-0067-49d3-ba96-9de6f2728e14',	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->groups()->post($requestRequestBody);


```