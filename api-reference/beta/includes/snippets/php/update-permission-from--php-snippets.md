---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Permission();


$requestRequestBody->setRoles(['read',]);
$result =  $graphClient->sitesById('site-id')->permissionsById('permission-id')->patch($requestRequestBody);


```