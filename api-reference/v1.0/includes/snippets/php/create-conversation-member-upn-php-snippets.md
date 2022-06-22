---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConversationMember();


$requestRequestBody->setVisibleHistoryStartDateTime(new DateTime("2019-04-18T23:51:43.255Z"));
$requestRequestBody->setRoles( [
'owner',],
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.aadUserConversationMember',
	"user@odata.bind" => 'https://graph.microsoft.com/v1.0/users/jacob@contoso.com',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->chatsById('chat-id')->members()->post($requestRequestBody);


```