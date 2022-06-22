---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SourceCollection();


$requestRequestBody->setDisplayName('Quarterly Financials search');
$requestRequestBody->setContentQuery('subject:\'Quarterly Financials\'');
$requestRequestBodyAdditionalData = [
	"custodianSources@odata.bind" =>  [
'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/custodians/2192ca408ea2410eba3bec8ae873be6b/userSources/46384443-4137-3032-3437-363939433735',	],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->sourceCollections()->post($requestRequestBody);


```