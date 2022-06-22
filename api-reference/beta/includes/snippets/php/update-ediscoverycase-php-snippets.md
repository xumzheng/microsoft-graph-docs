---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EdiscoveryCase();


$requestRequestBody->setDisplayName('My Case 1 - Renamed');
$requestRequestBody->setDescription('Updated description');
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->patch($requestRequestBody);


```