---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PrintTaskTrigger();


$requestRequestBody->setEvent(new PrintEvent('jobStarted'));
$requestRequestBodyAdditionalData = [
	"definition@odata.bind" => 'https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->print()->printersById('printer-id')->taskTriggers()->post($requestRequestBody);


```