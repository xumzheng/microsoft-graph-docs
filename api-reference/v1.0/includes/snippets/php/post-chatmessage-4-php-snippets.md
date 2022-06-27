---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new ChatMessage();



$body = new ItemBody();
$requestRequestBody->setBody($body);


$body->setContentType(new BodyType('html'));
$body->setContent('Here\'s the latest budget. <attachment id="153fa47d-18c9-4179-be08-9879815a9f90"></attachment>');

$attachmentsArray = [];

$attachmentsattachments1 = new ChatMessageAttachment();

$attachmentsattachments1->setId('153fa47d-18c9-4179-be08-9879815a9f90');
$attachmentsattachments1->setContentType('reference');
$attachmentsattachments1->setContentUrl('https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx');
$attachmentsattachments1->setName('Budget.docx');

$attachmentsArray []= $attachmentsattachments1;
$requestRequestBody->setAttachments($attachmentsArray);
$result =  $graphClient->teamsById('team-id')->channelsById('channel-id')->messages()->post($requestRequestBody);


```