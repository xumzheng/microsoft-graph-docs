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

$recipientsrecipients1 = new TeamworkNotificationRecipient();

$recipientsrecipients1AdditionalData = [
"@odata.type" => 'microsoft.graph.aadUserNotificationRecipient',
"userId" => '569363e2-4e49-4661-87f2-16f245c5d66a',
];
$recipientsrecipients1->setAdditionalData($recipientsrecipients1AdditionalData);

$recipientsArray []= $recipientsrecipients1;

$recipientsrecipients2 = new TeamworkNotificationRecipient();

$recipientsrecipients2AdditionalData = [
"@odata.type" => 'microsoft.graph.aadUserNotificationRecipient',
"userId" => 'ab88234e-0874-477c-9638-d144296ed04f',
];
$recipientsrecipients2->setAdditionalData($recipientsrecipients2AdditionalData);

$recipientsArray []= $recipientsrecipients2;

$recipientsrecipients3 = new TeamworkNotificationRecipient();

$recipientsrecipients3AdditionalData = [
"@odata.type" => 'microsoft.graph.aadUserNotificationRecipient',
"userId" => '01c64f53-69aa-42c7-9b7f-9f75195d6bfc',
];
$recipientsrecipients3->setAdditionalData($recipientsrecipients3AdditionalData);

$recipientsArray []= $recipientsrecipients3;
$requestRequestBody->setRecipients($recipientsArray);
$templateParametersArray = [];

$templateParameterstemplateParameters1 = new KeyValuePair();

$templateParameterstemplateParameters1->setName('pendingRequestCount');
$templateParameterstemplateParameters1->setValue('5');

$templateParametersArray []= $templateParameterstemplateParameters1;
$requestRequestBody->setTemplateParameters($templateParametersArray);
$result =  $graphClient->teamwork()->sendActivityNotificationToRecipients()->post($requestRequestBody);


```