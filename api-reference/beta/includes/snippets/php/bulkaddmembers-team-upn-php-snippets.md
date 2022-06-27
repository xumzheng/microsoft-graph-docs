---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ValuesRequestBody();


$valuesArray = [];

$valuesvalues1 = new ConversationMember();

$valuesvalues1AdditionalData = [
	"@odata.type" => 'microsoft.graph.aadUserConversationMember',
	"roles" => [],
"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')',
];
$valuesvalues1->setAdditionalData($valuesvalues1AdditionalData);

$valuesArray []= $valuesvalues1;

$valuesvalues2 = new ConversationMember();

$valuesvalues2AdditionalData = [
"@odata.type" => 'microsoft.graph.aadUserConversationMember',
"roles" => ['owner',],
"user@odata.bind" => 'https://graph.microsoft.com/beta/users(\'alex@contoso.com\')',
];
$valuesvalues2->setAdditionalData($valuesvalues2AdditionalData);

$valuesArray []= $valuesvalues2;
$requestRequestBody->setValues($valuesArray);
$result =  $graphClient->teamsById('team-id')->members()->add()->post($requestRequestBody);


```