---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrinterShare();


$requestRequestBody->setDisplayName('ShareName');
$requestRequestBody->setAllowAllUsers(False);
$requestRequestBodyAdditionalData = [
	"printer@odata.bind" => 'https://graph.microsoft.com/v1.0/print/printers/{printerId}',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->print()->shares()->post($requestRequestBody);


```