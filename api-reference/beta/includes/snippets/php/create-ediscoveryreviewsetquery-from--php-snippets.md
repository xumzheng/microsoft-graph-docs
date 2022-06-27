---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EdiscoveryReviewSetQuery();


$requestRequestBody->setDisplayName('My Query 1');
$requestRequestBody->setContentQuery('(Author="edison")');
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->reviewSetsById('ediscoveryReviewSet-id')->queries()->post($requestRequestBody);


```