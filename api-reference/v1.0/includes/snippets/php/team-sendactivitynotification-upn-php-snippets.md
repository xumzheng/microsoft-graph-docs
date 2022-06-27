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

$templateParameterstemplateParameters1 = new KeyValuePair();

$templateParameterstemplateParameters1->setName('reservationId');
$templateParameterstemplateParameters1->setValue('TREEE433');

$templateParametersArray []= $templateParameterstemplateParameters1;

$templateParameterstemplateParameters2 = new KeyValuePair();

$templateParameterstemplateParameters2->setName('currentSlot');
$templateParameterstemplateParameters2->setValue('23');

$templateParametersArray []= $templateParameterstemplateParameters2;
$requestRequestBody->setTemplateParameters($templateParametersArray);
$result =  $graphClient->teamsById('team-id')->sendActivityNotification()->post($requestRequestBody);


```