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
$topic->setValue('https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}');

$requestRequestBody->setActivityType('reservationUpdated');

$previewText = new ItemBody();
$requestRequestBody->setPreviewText($previewText);


$previewText->setContent('You have moved up the queue');


$recipient = new TeamworkNotificationRecipient();
$requestRequestBody->setRecipient($recipient);


$recipientAdditionalData = [
"@odata.type" => 'Microsoft.Teams.GraphSvc.aadUserNotificationRecipient',
"userId" => '569363e2-4e49-4661-87f2-16f245c5d66a',
];
$recipient->setAdditionalData($recipientAdditionalData);

$templateParametersArray = [];

$templateParameters1 = new KeyValuePair();

$templateParameters1->setName('reservationId');
$templateParameters1->setValue('TREEE433');

$templateParametersArray []= $templateParameters1;

$templateParameters2 = new KeyValuePair();

$templateParameters2->setName('currentSlot');
$templateParameters2->setValue('23');

$templateParametersArray []= $templateParameters2;
$requestRequestBody->setTemplateParameters($templateParametersArray);
$result =  $graphClient->teamsById('team-id')->sendActivityNotification()->post($requestRequestBody);


```