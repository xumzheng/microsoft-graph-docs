---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Custodian();


$requestRequestBody->setApplyHoldToSources('false');
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->custodiansById('custodian-id')->patch($requestRequestBody);


```