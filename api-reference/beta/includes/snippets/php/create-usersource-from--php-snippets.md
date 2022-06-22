---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UserSource();


$requestRequestBody->setEmail('admin@M365x809305.onmicrosoft.com');
$requestRequestBody->setIncludedSources(new SourceType('mailbox, site'));
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->legalHoldsById('ediscoveryHoldPolicy-id')->userSources()->post($requestRequestBody);


```