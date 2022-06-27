---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SendActivityNotificationPostRequestBody();



$topic = new TeamworkActivityTopic();
$requestRequestBody->setTopic($topic);


$topic->setSource(new TeamworkActivityTopicSource('entityUrl'));
$topic->setValue('https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}');

$requestRequestBody->setActivityType('approvalRequired');

$previewText = new ItemBody();
$requestRequestBody->setPreviewText($previewText);


$previewText->setContent('Deployment requires your approval');


$recipient = new TeamworkNotificationRecipient();
$requestRequestBody->setRecipient($recipient);


$recipientAdditionalData = [
"@odata.type" => 'Microsoft.Teams.GraphSvc.aadUserNotificationRecipient',
"userId" => 'jacob@contoso.com',
];
$recipient->setAdditionalData($recipientAdditionalData);

$templateParametersArray = [];

$templateParameterstemplateParameters1 = new KeyValuePair();

$templateParameterstemplateParameters1->setName('approvalTaskId');
$templateParameterstemplateParameters1->setValue('2020AAGGTAPP');

$templateParametersArray []= $templateParameterstemplateParameters1;
$requestRequestBody->setTemplateParameters($templateParametersArray);
$result =  $graphClient->chatsById('chat-id')->sendActivityNotification()->post($requestRequestBody);


```