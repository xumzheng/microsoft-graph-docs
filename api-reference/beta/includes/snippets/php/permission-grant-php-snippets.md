---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new GrantPostRequestBody();


$recipientsArray = [];

$recipientsrecipients1 = new DriveRecipient();

$recipientsrecipients1->setEmail('john@contoso.com');

$recipientsArray []= $recipientsrecipients1;

$recipientsrecipients2 = new DriveRecipient();

$recipientsrecipients2->setEmail('ryan@external.com');

$recipientsArray []= $recipientsrecipients2;
$requestRequestBody->setRecipients($recipientsArray);
$requestRequestBody->setRoles(['read',]);
$result =  $graphClient->sharesById('sharedDriveItem-id')->permission()->grant()->post($requestRequestBody);


```