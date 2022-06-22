---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SendMailPostRequestBody();



$message = new Message();
$requestRequestBody->setMessage($message);


$message->setSubject('9/9/2018: concert');

$body = new ItemBody();
$message->setBody($body);


$body->setContentType(new BodyType('HTML'));
$body->setContent('The group represents Nevada.');

$toRecipientsArray = [];

$toRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('AlexW@contoso.OnMicrosoft.com');


$toRecipientsArray []= $toRecipients1;
$message->setToRecipients($toRecipientsArray);
$internetMessageHeadersArray = [];

$internetMessageHeaders1 = new InternetMessageHeader();

$internetMessageHeaders1->setName('x-custom-header-group-name');
$internetMessageHeaders1->setValue('Nevada');

$internetMessageHeadersArray []= $internetMessageHeaders1;

$internetMessageHeaders2 = new InternetMessageHeader();

$internetMessageHeaders2->setName('x-custom-header-group-id');
$internetMessageHeaders2->setValue('NV001');

$internetMessageHeadersArray []= $internetMessageHeaders2;
$message->setInternetMessageHeaders($internetMessageHeadersArray);

$result =  $graphClient->me()->sendMail()->post($requestRequestBody);


```