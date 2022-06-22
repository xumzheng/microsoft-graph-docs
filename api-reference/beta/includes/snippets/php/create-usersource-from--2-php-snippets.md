---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UserSource();


$requestRequestBody->setEmail('adelev@contoso.com');
$requestRequestBody->setIncludedSources(new SourceType('mailbox'));
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->legalHoldsById('legalHold-id')->userSources()->post($requestRequestBody);


```