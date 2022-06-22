---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CreateForwardPostRequestBody();



$message = new Message();
$requestRequestBody->setMessage($message);


$message->setIsDeliveryReceiptRequested(True);
$toRecipientsArray = [];

$toRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('danas@contoso.onmicrosoft.com');
$emailAddress->setName('Dana Swope');


$toRecipientsArray []= $toRecipients1;
$message->setToRecipients($toRecipientsArray);

$requestRequestBody->setComment('Dana, just want to make sure you get this; you\'ll need this if the project gets approved.');
$result =  $graphClient->me()->messagesById('message-id')->createForward()->post($requestRequestBody);


```