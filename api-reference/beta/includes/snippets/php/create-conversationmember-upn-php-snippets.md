---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ConversationMember();


$requestRequestBody->setRoles( [
'owner',],
$requestRequestBodyAdditionalData = [
	"@odata.type" => '#microsoft.graph.aadUserConversationMember',
	"user@odata.bind" => 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')',
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->teamsById('team-id')->members()->post($requestRequestBody);


```