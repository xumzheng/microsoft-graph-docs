---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new LegalHold();


$requestRequestBody->setDescription('This is a description for a legalHold');
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->legalHoldsById('legalHold-id')->patch($requestRequestBody);


```