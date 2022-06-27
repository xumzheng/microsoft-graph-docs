---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Subscription();


$requestRequestBody->setChangeType('created');
$requestRequestBody->setNotificationUrl('https://webhook.azurewebsites.net/api/send/myNotifyClient');
$requestRequestBody->setResource('me/mailFolders(\'Inbox\')/messages');
$requestRequestBody->setExpirationDateTime(new DateTime("2016-11-20T18:23:45.9356913Z"));
$requestRequestBody->setClientState('secretClientValue');
$requestRequestBody->setLatestSupportedTlsVersion('v1_2');
$result =  $graphClient->subscriptions()->post($requestRequestBody);


```