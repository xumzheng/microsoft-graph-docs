---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new LegalHold();


$requestRequestBody->setDescription('String');

$createdBy = new IdentitySet();
$requestRequestBody->setCreatedBy($createdBy);


$createdByAdditionalData = [
	"@odata.type" => 'microsoft.graph.identitySet',
];
$createdBy->setAdditionalData($createdByAdditionalData);

$requestRequestBody->setIsEnabled('Boolean');
$requestRequestBody->setStatus(new LegalHoldStatus('String'));
$requestRequestBody->setContentQuery('String');
$requestRequestBody->setErrors( [
'String',],
$requestRequestBody->setDisplayName('String');
$requestRequestBodyAdditionalData = [
"@odata.type" => '#microsoft.graph.ediscovery.legalHold',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->legalHolds()->post($requestRequestBody);


```