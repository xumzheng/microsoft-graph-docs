---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new PersonAnnotation();



$detail = new ItemBody();
$requestRequestBody->setDetail($detail);


$detail->setContentType(new BodyType('text'));
$detail->setContent('I am originally from Australia, but grew up in Moscow, Russia.');

$requestRequestBody->setDisplayName('About Me');
$result =  $graphClient->me()->profile()->notes()->post($requestRequestBody);


```