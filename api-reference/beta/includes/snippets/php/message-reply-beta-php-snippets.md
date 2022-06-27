---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReplyPostRequestBody();



$message = new Message();
$requestRequestBody->setMessage($message);


$toRecipientsArray = [];

$toRecipientstoRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipientstoRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('samanthab@contoso.onmicrosoft.com');
$emailAddress->setName('Samantha Booth');


$toRecipientsArray []= $toRecipientstoRecipients1;

$toRecipientstoRecipients2 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipientstoRecipients2->setEmailAddress($emailAddress);


$emailAddress->setAddress('randiw@contoso.onmicrosoft.com');
$emailAddress->setName('Randi Welch');


$toRecipientsArray []= $toRecipientstoRecipients2;
$message->setToRecipients($toRecipientsArray);

$requestRequestBody->setComment('Samantha, Randi, would you name the group please?');
$result =  $graphClient->me()->messagesById('message-id')->reply()->post($requestRequestBody);


```