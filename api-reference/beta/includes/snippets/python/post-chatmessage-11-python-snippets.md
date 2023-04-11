---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.subject = 'Announcement Subheading'

body = ItemBody()
body.ContentType(BodyType('text'))

body.content = '<attachment id=\"d7ddbf876ae340c3a03bada395ec7da7\"></attachment>Announcement text'


request_body.body = body
attachmentsChatMessageAttachment1 = ChatMessageAttachment()
attachmentsChatMessageAttachment1.id = 'd7ddbf876ae340c3a03bada395ec7da7'

attachmentsChatMessageAttachment1.contentType = 'application/vnd.microsoft.teams.messaging-announcementBanner'

attachmentsChatMessageAttachment1.contentUrl=null

attachmentsChatMessageAttachment1.content = '{\"title\":\"Announcement heading\",\"cardImageType\":\"uploadedImage\",\"cardImageDetails\":{\"uploadedImageDetail\":{\"originalImage\":{\"source\":\"../hostedContents/1/$value\",\"width\":1379,\"height\":268,\"croppedWidth\":918.0,\"croppedHeight\":178.4075416968818,\"leftMargin\":0.0,\"topMargin\":90.7962291515591,\"imageContentType\":\"image/png\"},\"croppedImage\":{\"source\":\"../hostedContents/2/$value\"}}}}'

attachmentsChatMessageAttachment1.name=null

attachmentsChatMessageAttachment1.thumbnailUrl=null


attachmentsArray []= attachmentsChatMessageAttachment1;
request_body.attachments(attachmentsArray)


hostedContentsChatMessageHostedContent1 = ChatMessageHostedContent()
hostedContentsChatMessageHostedContent1.ContentBytes(base64_decode('iVBORw0KGgoAAAANSUhEUgAABWMAAAEMCAYAAAChuaTsAAAAAXNSR0IArs4c6QAAAARnQU1BA'))

hostedContentsChatMessageHostedContent1.contentType = 'image/png'

additionalData = [
'@microsoft.graph.temporaryId' => '1', 
];
hostedContentsChatMessageHostedContent1.additionaldata(additionalData)



hostedContentsArray []= hostedContentsChatMessageHostedContent1;
hostedContentsChatMessageHostedContent2 = ChatMessageHostedContent()
hostedContentsChatMessageHostedContent2.ContentBytes(base64_decode('iVBORw0KGgoAAAANSUhEUgAAA5YAAAB4CAYAAACJrW0RAAAAAXNSR0IArs4c6QAAIABJREFUe'))

hostedContentsChatMessageHostedContent2.contentType = 'image/png'

additionalData = [
'@microsoft.graph.temporaryId' => '2', 
];
hostedContentsChatMessageHostedContent2.additionaldata(additionalData)



hostedContentsArray []= hostedContentsChatMessageHostedContent2;
request_body.hostedcontents(hostedContentsArray)




request_configuration = MessagesRequestBuilderPostRequestConfiguration(
)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body = request_body)


```