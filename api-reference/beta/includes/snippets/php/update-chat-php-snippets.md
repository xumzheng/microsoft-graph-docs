---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new Chat();


$requestRequestBody->setTopic('Group chat title update');
$result =  $graphClient->chatsById('chat-id')->patch($requestRequestBody);


```