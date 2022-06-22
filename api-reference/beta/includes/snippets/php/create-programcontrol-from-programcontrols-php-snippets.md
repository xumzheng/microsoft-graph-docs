---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ProgramControl();


$requestRequestBody->setControlId('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213');
$requestRequestBody->setControlTypeId('6e4f3d20-c5c3-407f-9695-8460952bcc68');
$requestRequestBody->setProgramId('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213');
$result =  $graphClient->programControls()->post($requestRequestBody);


```