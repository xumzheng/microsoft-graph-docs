---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new CommentRequestBody();


$requestRequestBody->setComment('Cancelling for this week due to all hands');
$result =  $graphClient->me()->eventsById('event-id')->cancel()->post($requestRequestBody);


```