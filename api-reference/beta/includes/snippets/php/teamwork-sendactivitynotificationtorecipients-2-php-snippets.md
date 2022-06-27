---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new SendActivityNotificationToRecipientsPostRequestBody();



$topic = new TeamworkActivityTopic();
$requestRequestBody->setTopic($topic);


$topic->setSource(new TeamworkActivityTopicSource('text'));
$topic->setValue('Deployment Approvals Channel');
$topic->setWebUrl('https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000');

$requestRequestBody->setActivityType('deploymentApprovalRequired');

$previewText = new ItemBody();
$requestRequestBody->setPreviewText($previewText);


$previewText->setContent('New deployment requires your approval');

$templateParametersArray = [];

$templateParameterstemplateParameters1 = new KeyValuePair();

$templateParameterstemplateParameters1->setName('deploymentId');
$templateParameterstemplateParameters1->setValue('6788662');

$templateParametersArray []= $templateParameterstemplateParameters1;
$requestRequestBody->setTemplateParameters($templateParametersArray);
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
$result =  $graphClient->teamwork()->sendActivityNotificationToRecipients()->post($requestRequestBody);


```