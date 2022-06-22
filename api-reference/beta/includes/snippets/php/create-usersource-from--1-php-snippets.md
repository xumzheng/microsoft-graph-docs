---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UserSource();


$requestRequestBody->setEmail('megan@contoso.com');
$requestRequestBody->setIncludedSources(new SourceType('mailbox, site'));
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->custodiansById('custodian-id')->userSources()->post($requestRequestBody);


```