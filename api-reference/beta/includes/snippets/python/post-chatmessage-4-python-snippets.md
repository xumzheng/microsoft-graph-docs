---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
body = ItemBody()
body.ContentType(BodyType('html'))

body.content = 'Here\'s the latest budget. <attachment id=\"153fa47d-18c9-4179-be08-9879815a9f90\"></attachment>'


request_body.body = body
attachments_chat_message_attachment1 = ChatMessageAttachment()
attachmentsChatMessageAttachment1.id = '153fa47d-18c9-4179-be08-9879815a9f90'

attachmentsChatMessageAttachment1.contentType = 'reference'

attachmentsChatMessageAttachment1.contentUrl = 'https://m365x987948.sharepoint.com/sites/test/Shared%20Documents/General/test%20doc.docx'

attachmentsChatMessageAttachment1.name = 'Budget.docx'


attachmentsArray []= attachmentsChatMessageAttachment1;
request_body.attachments(attachmentsArray)





result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body = request_body)


```