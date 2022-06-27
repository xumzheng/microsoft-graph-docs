---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AdministrativeUnit();


$requestRequestBody->setDisplayName('Seattle District Technical Schools');
$requestRequestBody->setDescription('Seattle district technical schools administration');
$requestRequestBody->setVisibility('HiddenMembership');
$result =  $graphClient->directory()->administrativeUnits()->post($requestRequestBody);


```