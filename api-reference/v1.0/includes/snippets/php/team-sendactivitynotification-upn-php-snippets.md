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
$topic->setValue('https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}');

$requestRequestBody->setActivityType('reservationUpdated');

$previewText = new ItemBody();
$requestRequestBody->setPreviewText($previewText);


$previewText->setContent('You have moved up the queue');


$recipient = new TeamworkNotificationRecipient();
$requestRequestBody->setRecipient($recipient);


$recipientAdditionalData = [
"@odata.type" => 'Microsoft.Teams.GraphSvc.aadUserNotificationRecipient',
"userId" => 'jacob@contoso.com',
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