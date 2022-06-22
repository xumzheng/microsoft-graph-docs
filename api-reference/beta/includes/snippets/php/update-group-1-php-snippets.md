---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Group();


$requestRequestBody->setDescription('Contoso Life v2.0');
$requestRequestBody->setDisplayName('Contoso Life Renewed');
$result =  $graphClient->groupsById('group-id')->patch($requestRequestBody);


```