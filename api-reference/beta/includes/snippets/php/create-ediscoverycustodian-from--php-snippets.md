---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EdiscoveryCustodian();


$requestRequestBody->setEmail('AdeleV@contoso.com');
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->custodians()->post($requestRequestBody);


```