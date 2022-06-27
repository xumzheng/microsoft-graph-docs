---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ForwardPostRequestBody();


$toRecipientsArray = [];

$toRecipientstoRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipientstoRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('danas@contoso.onmicrosoft.com');
$emailAddress->setName('Dana Swope');


$toRecipientsArray []= $toRecipientstoRecipients1;
$requestRequestBody->setToRecipients($toRecipientsArray);
$requestRequestBody->setComment('Dana, hope you can make this meeting.');
$result =  $graphClient->me()->eventsById('event-id')->forward()->post($requestRequestBody);


```