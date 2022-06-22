---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ValuesRequestBody();


$valuesArray = [];

$values1 = new ConversationMember();

$values1AdditionalData = [
		"@odata.type" => 'microsoft.graph.aadUserConversationMember',
		"roles" =>  [
		],
		"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'18a80140-b0fb-4489-b360-2f6efaf225a0\')',
	];
$values1->setAdditionalData($values1AdditionalData);

$valuesArray []= $values1;

$values2 = new ConversationMember();

$values2AdditionalData = [
	"@odata.type" => 'microsoft.graph.aadUserConversationMember',
	"roles" =>  [
'owner',	],
	"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'86503198-b81b-43fe-81ee-ad45b8848ac9\')',
];
$values2->setAdditionalData($values2AdditionalData);

$valuesArray []= $values2;
$requestRequestBody->setValues($valuesArray);
$result =  $graphClient->teamsById('team-id')->members()->add()->post($requestRequestBody);


```