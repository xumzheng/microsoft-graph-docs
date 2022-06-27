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

$toRecipientstoRecipients1 = new Recipient();


$emailAddress = new EmailAddress();
$toRecipientstoRecipients1->setEmailAddress($emailAddress);


$emailAddress->setAddress('AlexW@contoso.OnMicrosoft.com');


$toRecipientsArray []= $toRecipientstoRecipients1;
$requestRequestBody->setToRecipients($toRecipientsArray);
$internetMessageHeadersArray = [];

$internetMessageHeadersinternetMessageHeaders1 = new InternetMessageHeader();

$internetMessageHeadersinternetMessageHeaders1->setName('x-custom-header-group-name');
$internetMessageHeadersinternetMessageHeaders1->setValue('Washington');

$internetMessageHeadersArray []= $internetMessageHeadersinternetMessageHeaders1;

$internetMessageHeadersinternetMessageHeaders2 = new InternetMessageHeader();

$internetMessageHeadersinternetMessageHeaders2->setName('x-custom-header-group-id');
$internetMessageHeadersinternetMessageHeaders2->setValue('WA001');

$internetMessageHeadersArray []= $internetMessageHeadersinternetMessageHeaders2;
$requestRequestBody->setInternetMessageHeaders($internetMessageHeadersArray);
$result =  $graphClient->me()->messages()->post($requestRequestBody);


```