---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new StorageLocationRequestBody();


$requestRequestBody->setStorageLocation('storageLocation-value');
$result =  $graphClient->usersById('user-id')->exportPersonalData()->post($requestRequestBody);


```