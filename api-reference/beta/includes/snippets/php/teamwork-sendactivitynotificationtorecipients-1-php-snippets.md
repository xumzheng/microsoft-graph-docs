---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SendActivityNotificationToRecipientsPostRequestBody();



$topic = new TeamworkActivityTopic();
$requestRequestBody->setTopic($topic);


$topic->setSource(new TeamworkActivityTopicSource('entityUrl'));
$topic->setValue('https://graph.microsoft.com/beta/appCatalogs/teamsApps/{teamsAppId}');

$requestRequestBody->setActivityType('pendingFinanceApprovalRequests');

$previewText = new ItemBody();
$requestRequestBody->setPreviewText($previewText);


$previewText->setContent('Internal spending team has a pending finance approval requests');

$recipientsArray = [];

$recipients1 = new TeamworkNotificationRecipient();

$recipients1AdditionalData = [
"@odata.type" => 'microsoft.graph.aadUserNotificationRecipient',
"userId" => '569363e2-4e49-4661-87f2-16f245c5d66a',
];
$recipients1->setAdditionalData($recipients1AdditionalData);

$recipientsArray []= $recipients1;

$recipients2 = new TeamworkNotificationRecipient();

$recipients2AdditionalData = [
"@odata.type" => 'microsoft.graph.aadUserNotificationRecipient',
"userId" => 'ab88234e-0874-477c-9638-d144296ed04f',
];
$recipients2->setAdditionalData($recipients2AdditionalData);

$recipientsArray []= $recipients2;

$recipients3 = new TeamworkNotificationRecipient();

$recipients3AdditionalData = [
"@odata.type" => 'microsoft.graph.aadUserNotificationRecipient',
"userId" => '01c64f53-69aa-42c7-9b7f-9f75195d6bfc',
];
$recipients3->setAdditionalData($recipients3AdditionalData);

$recipientsArray []= $recipients3;
$requestRequestBody->setRecipients($recipientsArray);
$templateParametersArray = [];

$templateParameters1 = new KeyValuePair();

$templateParameters1->setName('pendingRequestCount');
$templateParameters1->setValue('5');

$templateParametersArray []= $templateParameters1;
$requestRequestBody->setTemplateParameters($templateParametersArray);
$result =  $graphClient->teamwork()->sendActivityNotificationToRecipients()->post($requestRequestBody);


```