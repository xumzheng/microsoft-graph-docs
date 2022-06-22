---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EdiscoveryReviewSet();


$requestRequestBody->setDisplayName('My review set 2');
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->reviewSets()->post($requestRequestBody);


```