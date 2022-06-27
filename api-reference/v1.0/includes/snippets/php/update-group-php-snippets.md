---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Group();


$requestRequestBody->setDescription('Library Assist');
$requestRequestBody->setDisplayName('Library Assist');
$requestRequestBody->setGroupTypes(['Unified',]);
$requestRequestBody->setMailEnabled(True);
$requestRequestBody->setMailNickname('library-help');
$result =  $graphClient->groupsById('group-id')->patch($requestRequestBody);


```