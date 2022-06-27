---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EdiscoveryCase();


$requestRequestBody->setDisplayName('CONTOSO LITIGATION-005');
$requestRequestBody->setDescription('Project Bazooka');
$requestRequestBody->setExternalId('324516');
$result =  $graphClient->security()->cases()->ediscoveryCases()->post($requestRequestBody);


```