---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AdministrativeUnit();


$requestRequestBody->setDisplayName('Greater Seattle District Technical Schools');
$result =  $graphClient->directory()->administrativeUnitsById('administrativeUnit-id')->patch($requestRequestBody);


```