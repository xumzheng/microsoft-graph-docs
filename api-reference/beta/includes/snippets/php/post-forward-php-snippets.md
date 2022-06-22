---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ForwardPostRequestBody();


$requestRequestBody->setComment('comment-value');
$toRecipientsArray = [];

$toRecipients1 = new Recipient();

$toRecipients1AdditionalData = [
	];
$toRecipients1->setAdditionalData($toRecipients1AdditionalData);

$toRecipientsArray []= $toRecipients1;
$requestRequestBody->setToRecipients($toRecipientsArray);
$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->postsById('post-id')->forward()->post($requestRequestBody);


```