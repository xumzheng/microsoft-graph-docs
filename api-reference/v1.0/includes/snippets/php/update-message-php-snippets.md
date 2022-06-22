---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Message();


$requestRequestBody->setSubject('subject-value');

$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType(new BodyType(''));
$body->setContent('content-value');

$requestRequestBody->setInferenceClassification(new InferenceClassificationType('other'));
$result =  $graphClient->me()->messagesById('message-id')->patch($requestRequestBody);


```