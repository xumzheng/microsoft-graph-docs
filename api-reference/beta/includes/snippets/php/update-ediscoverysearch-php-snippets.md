---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EdiscoverySearch();


$requestRequestBody->setDisplayName('Teams search');
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->searchesById('ediscoverySearch-id')->patch($requestRequestBody);


```