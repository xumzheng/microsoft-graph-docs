---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new UnifiedGroupSource();


$requestRequestBody->setIncludedSources(new SourceType('mailbox, site'));
$requestRequestBodyAdditionalData = [
	"group@odata.bind" => 'https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->custodiansById('custodian-id')->unifiedGroupSources()->post($requestRequestBody);


```