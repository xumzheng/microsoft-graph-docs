---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CreateUploadSessionPostRequestBody();
$attachmentInfo = new AttachmentInfo();
$attachmentInfo->setAttachmentType(new AttachmentType('file'));

$attachmentInfo->setName('flower');

$attachmentInfo->setSize(3483322);


$requestBody->setAttachmentInfo($attachmentInfo);


$requestResult = $graphServiceClient->me()->todo()->listsById('todoTaskList-id')->tasksById('todoTask-id')->attachments()->createUploadSession()->post($requestBody);


```