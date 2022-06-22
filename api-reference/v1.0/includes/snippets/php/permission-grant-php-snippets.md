---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GrantPostRequestBody();


$recipientsArray = [];

$recipients1 = new DriveRecipient();

$recipients1->setEmail('john@contoso.com');

$recipientsArray []= $recipients1;

$recipients2 = new DriveRecipient();

$recipients2->setEmail('ryan@external.com');

$recipientsArray []= $recipients2;
$requestRequestBody->setRecipients($recipientsArray);
$requestRequestBody->setRoles( [
'read',],
$result =  $graphClient->sharesById('sharedDriveItem-id')->permission()->grant()->post($requestRequestBody);


```