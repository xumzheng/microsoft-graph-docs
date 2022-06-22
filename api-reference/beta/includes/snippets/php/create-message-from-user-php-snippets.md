---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Message();


$requestRequestBody->setSubject('Did you see last night\'s game?');
$requestRequestBody->setImportance(new Importance('Low'));

$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType(new BodyType('HTML'));
$body->setContent('They were <b>awesome</b>!');

$toRecipientsArray = [];

$toRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('AdeleV@contoso.onmicrosoft.com');


$toRecipientsArray []= $toRecipients1;
$requestRequestBody->setToRecipients($toRecipientsArray);
$result =  $graphClient->me()->messages()->post($requestRequestBody);


```