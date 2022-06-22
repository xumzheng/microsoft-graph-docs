---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrinterShare();


$requestRequestBody->setDisplayName('ShareName');
$requestRequestBody->setAllowAllUsers(True);
$requestRequestBodyAdditionalData = [
	"printer@odata.bind" => 'https://graph.microsoft.com/beta/print/printers/{id}',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->print()->sharesById('printerShare-id')->patch($requestRequestBody);


```