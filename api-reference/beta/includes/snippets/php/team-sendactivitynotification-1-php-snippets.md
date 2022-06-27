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
$topic->setValue('https://graph.microsoft.com/beta/teams/{teamId}');

$requestRequestBody->setActivityType('pendingFinanceApprovalRequests');

$previewText = new ItemBody();
$requestRequestBody->setPreviewText($previewText);


$previewText->setContent('Internal spending team has a pending finance approval requests');


$recipient = new TeamworkNotificationRecipient();
$requestRequestBody->setRecipient($recipient);


$recipientAdditionalData = [
"@odata.type" => 'microsoft.graph.aadUserNotificationRecipient',
"userId" => '569363e2-4e49-4661-87f2-16f245c5d66a',
];
$recipient->setAdditionalData($recipientAdditionalData);

$templateParametersArray = [];

$templateParameterstemplateParameters1 = new KeyValuePair();

$templateParameterstemplateParameters1->setName('pendingRequestCount');
$templateParameterstemplateParameters1->setValue('5');

$templateParametersArray []= $templateParameterstemplateParameters1;
$requestRequestBody->setTemplateParameters($templateParametersArray);
$result =  $graphClient->teamsById('team-id')->sendActivityNotification()->post($requestRequestBody);


```