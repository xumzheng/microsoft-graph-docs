---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SendMailPostRequestBody();



$message = new Message();
$requestRequestBody->setMessage($message);


$message->setSubject('Project kickoff');
$toRecipientsArray = [];

$toRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipients1->setEmailAddress($emailAddress);


$emailAddress->setName('Samantha Booth');
$emailAddress->setAddress('samanthab@contoso.onmicrosoft.com');


$toRecipientsArray []= $toRecipients1;
$message->setToRecipients($toRecipientsArray);
$mentionsArray = [];

$mentions1 = new Mention();


$mentioned = new EmailAddress();
$mentions1->setMentioned($mentioned);


$mentioned->setName('Dana Swope');
$mentioned->setAddress('danas@contoso.onmicrosoft.com');


$mentionsArray []= $mentions1;
$message->setMentions($mentionsArray);

$result =  $graphClient->me()->sendMail()->post($requestRequestBody);


```