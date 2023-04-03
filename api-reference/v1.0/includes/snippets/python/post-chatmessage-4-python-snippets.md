---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ChatMessage();
body = ItemBody();
body.setContentType(BodyType('html'));

body.setContent('Here\'s the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>');


requestBody.setBody($body);
attachmentsChatMessageAttachment1 = ChatMessageAttachment();
attachmentsChatMessageAttachment1.setId('153fa47d-18c9-4179-be08-9879815a9f90');

attachmentsChatMessageAttachment1.setContentType('reference');

attachmentsChatMessageAttachment1.setContentUrl('https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx');

attachmentsChatMessageAttachment1.setName('Budget.docx');


attachmentsArray []= attachmentsChatMessageAttachment1;
requestBody.setAttachments(attachmentsArray);




requestResult = graphServiceClient.teamsById('team-id').channelsById('channel-id').messages().post(requestBody);


```