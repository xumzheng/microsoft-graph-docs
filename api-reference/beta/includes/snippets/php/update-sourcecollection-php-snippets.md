---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SourceCollection();


$requestRequestBody->setDisplayName('Quarterly Financials search');
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->sourceCollectionsById('sourceCollection-id')->patch($requestRequestBody);


```