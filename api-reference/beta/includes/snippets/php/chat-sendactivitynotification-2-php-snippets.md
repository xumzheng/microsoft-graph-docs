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
$topic->setValue('https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}');

$requestRequestBody->setActivityType('approvalRequired');

$previewText = new ItemBody();
$requestRequestBody->setPreviewText($previewText);


$previewText->setContent('Deployment requires your approval');


$recipient = new TeamworkNotificationRecipient();
$requestRequestBody->setRecipient($recipient);


$recipientAdditionalData = [
"@odata.type" => 'Microsoft.Teams.GraphSvc.aadUserNotificationRecipient',
"userId" => '569363e2-4e49-4661-87f2-16f245c5d66a',
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