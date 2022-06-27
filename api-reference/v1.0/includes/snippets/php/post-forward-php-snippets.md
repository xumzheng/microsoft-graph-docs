---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ForwardPostRequestBody();


$requestRequestBody->setComment('comment-value');
$toRecipientsArray = [];

$toRecipientstoRecipients1 = new Recipient();

$toRecipientstoRecipients1AdditionalData = [
];
$toRecipientstoRecipients1->setAdditionalData($toRecipientstoRecipients1AdditionalData);

$toRecipientsArray []= $toRecipientstoRecipients1;
$requestRequestBody->setToRecipients($toRecipientsArray);
$result =  $graphClient->groupsById('group-id')->threadsById('conversationThread-id')->postsById('post-id')->forward()->post($requestRequestBody);


```