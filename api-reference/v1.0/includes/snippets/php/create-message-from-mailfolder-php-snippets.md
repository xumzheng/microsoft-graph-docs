---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Message();


$requestRequestBody->setReceivedDateTime(new DateTime("datetime-value"));
$requestRequestBody->setSentDateTime(new DateTime("datetime-value"));
$requestRequestBody->setHasAttachments(True);
$requestRequestBody->setSubject('subject-value');

$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType(new BodyType(''));
$body->setContent('content-value');

$requestRequestBody->setBodyPreview('bodyPreview-value');
$result =  $graphClient->me()->mailFoldersById('mailFolder-id')->messages()->post($requestRequestBody);


```