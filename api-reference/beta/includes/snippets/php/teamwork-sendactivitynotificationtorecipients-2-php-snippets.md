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

$templateParameters1 = new KeyValuePair();

$templateParameters1->setName('deploymentId');
$templateParameters1->setValue('6788662');

$templateParametersArray []= $templateParameters1;
$requestRequestBody->setTemplateParameters($templateParametersArray);
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
$result =  $graphClient->teamwork()->sendActivityNotificationToRecipients()->post($requestRequestBody);


```