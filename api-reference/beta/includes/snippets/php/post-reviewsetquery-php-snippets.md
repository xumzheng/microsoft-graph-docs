---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReviewSetQuery();


$requestRequestBody->setDisplayName('My Query 1');
$requestRequestBody->setQuery('(subject:"Quarterly Financials")');
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->reviewSetsById('reviewSet-id')->queries()->post($requestRequestBody);


```