---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Custodian();


$requestRequestBody->setEmail('AdeleV@contoso.com');
$requestRequestBody->setApplyHoldToSources('true');
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->custodians()->post($requestRequestBody);


```