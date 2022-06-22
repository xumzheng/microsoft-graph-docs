---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ReplyAllPostRequestBody();


$requestRequestBody->setComment('comment-value');
$result =  $graphClient->me()->messagesById('message-id')->replyAll()->post($requestRequestBody);


```