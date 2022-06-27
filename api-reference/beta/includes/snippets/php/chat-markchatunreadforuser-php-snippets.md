---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new MarkChatUnreadForUserPostRequestBody();



$user = new TeamworkUserIdentity();
$requestRequestBody->setUser($user);


$user->setId('d864e79f-a516-4d0f-9fee-0eeb4d61fdc2');

$requestRequestBody->setTenantId('2a690434-97d9-4eed-83a6-f5f13600199a');
$requestRequestBody->setLastMessageReadDateTime(new DateTime("2021-05-27T22:13:01.577Z"));
$result =  $graphClient->chatsById('chat-id')->markChatUnreadForUser()->post($requestRequestBody);


```