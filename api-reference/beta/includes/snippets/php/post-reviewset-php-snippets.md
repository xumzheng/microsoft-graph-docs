---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReviewSet();


$requestRequestBody->setDisplayName('My Reviewset 3');
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->reviewSets()->post($requestRequestBody);


```