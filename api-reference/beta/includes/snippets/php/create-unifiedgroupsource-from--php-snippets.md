---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedGroupSource();


$requestRequestBody->setIncludedSources(new SourceType('mailbox'));
$requestRequestBodyAdditionalData = [
	"group@odata.bind" => 'https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->security()->cases()->ediscoveryCasesById('ediscoveryCase-id')->custodiansById('ediscoveryCustodian-id')->unifiedGroupSources()->post($requestRequestBody);


```