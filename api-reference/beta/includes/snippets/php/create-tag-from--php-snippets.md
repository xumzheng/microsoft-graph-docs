---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Tag();


$requestRequestBody->setDisplayName('Privileged');
$requestRequestBody->setDescription('The document is privileged');
$requestRequestBodyAdditionalData = [
	"parent@odata.bind" => 'https://graph.microsoft.com/beta/compliance/ediscovery/cases/47746044-fd0b-4a30-acfc-5272b691ba5b/tags/98fdad78bbce4519b75474bc150575c3',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->compliance()->ediscovery()->casesById('case-id')->tags()->post($requestRequestBody);


```