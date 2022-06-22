---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConversationMember();


$requestRequestBody->setRoles( [
],
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.aadUserConversationMember',
	"user@odata.bind" => 'https://graph.microsoft.com/beta/users/bc3598dd-cce4-4742-ae15-173429951408',
	"tenantId" => 'a18103d1-a6ef-4f66-ac64-e4ef42ea8681',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->members()->post($requestRequestBody);


```