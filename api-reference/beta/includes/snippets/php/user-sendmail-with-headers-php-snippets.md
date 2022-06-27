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

$toRecipientstoRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipientstoRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('AlexW@contoso.OnMicrosoft.com');


$toRecipientsArray []= $toRecipientstoRecipients1;
$message->setToRecipients($toRecipientsArray);
$internetMessageHeadersArray = [];

$internetMessageHeadersinternetMessageHeaders1 = new InternetMessageHeader();

$internetMessageHeadersinternetMessageHeaders1->setName('x-custom-header-group-name');
$internetMessageHeadersinternetMessageHeaders1->setValue('Nevada');

$internetMessageHeadersArray []= $internetMessageHeadersinternetMessageHeaders1;

$internetMessageHeadersinternetMessageHeaders2 = new InternetMessageHeader();

$internetMessageHeadersinternetMessageHeaders2->setName('x-custom-header-group-id');
$internetMessageHeadersinternetMessageHeaders2->setValue('NV001');

$internetMessageHeadersArray []= $internetMessageHeadersinternetMessageHeaders2;
$message->setInternetMessageHeaders($internetMessageHeadersArray);

$result =  $graphClient->me()->sendMail()->post($requestRequestBody);


```