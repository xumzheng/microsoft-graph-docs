---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Message();


$requestRequestBody->setSubject('9/8/2018: concert');

$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType(new BodyType('HTML'));
$body->setContent('The group represents Washington.');

$toRecipientsArray = [];

$toRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('AlexW@contoso.OnMicrosoft.com');


$toRecipientsArray []= $toRecipients1;
$requestRequestBody->setToRecipients($toRecipientsArray);
$internetMessageHeadersArray = [];

$internetMessageHeaders1 = new InternetMessageHeader();

$internetMessageHeaders1->setName('x-custom-header-group-name');
$internetMessageHeaders1->setValue('Washington');

$internetMessageHeadersArray []= $internetMessageHeaders1;

$internetMessageHeaders2 = new InternetMessageHeader();

$internetMessageHeaders2->setName('x-custom-header-group-id');
$internetMessageHeaders2->setValue('WA001');

$internetMessageHeadersArray []= $internetMessageHeaders2;
$requestRequestBody->setInternetMessageHeaders($internetMessageHeadersArray);
$result =  $graphClient->me()->messages()->post($requestRequestBody);


```