---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SelfActivatePostRequestBody();


$requestRequestBody->setReason('reason-value');
$requestRequestBody->setDuration('duration-value');
$requestRequestBody->setTicketNumber('ticketNumber-value');
$requestRequestBody->setTicketSystem('ticketSystem-value');
$result =  $graphClient->privilegedRolesById('privilegedRole-id')->selfActivate()->post($requestRequestBody);


```