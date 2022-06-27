---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrinterShare();


$requestRequestBody->setName('name-value');
$requestRequestBodyAdditionalData = [
	"printer@odata.bind" => 'https://graph.microsoft.com/beta/print/printers/{id}',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->print()->shares()->post($requestRequestBody);


```