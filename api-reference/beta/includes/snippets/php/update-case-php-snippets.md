---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Case();


$requestRequestBody->setDisplayName('My Case 1 - Renamed');
$requestRequestBody->setDescription('Updated description');
$requestRequestBody->setExternalId('Updated externalId');
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->patch($requestRequestBody);


```