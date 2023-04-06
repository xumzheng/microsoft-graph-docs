---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.setSubject('Announcement Subheading')

body = ItemBody()
body.setContentType(BodyType('text'))

body.setContent('<attachment id=\"d7ddbf876ae340c3a03bada395ec7da7\"></attachment>Announcement text')


request_body.setBody($body)
attachmentsChatMessageAttachment1 = ChatMessageAttachment()
attachmentsChatMessageAttachment1.setId('d7ddbf876ae340c3a03bada395ec7da7')

attachmentsChatMessageAttachment1.setContentType('application/vnd.microsoft.teams.messaging-announcementBanner')

attachmentsChatMessageAttachment1.setContentUrl(null)

attachmentsChatMessageAttachment1.setContent('{\"title\":\"Announcement heading\",\"cardImageType\":\"uploadedImage\",\"cardImageDetails\":{\"uploadedImageDetail\":{\"originalImage\":{\"source\":\"../hostedContents/1/$value\",\"width\":1379,\"height\":268,\"croppedWidth\":918.0,\"croppedHeight\":178.4075416968818,\"leftMargin\":0.0,\"topMargin\":90.7962291515591,\"imageContentType\":\"image/png\"},\"croppedImage\":{\"source\":\"../hostedContents/2/$value\"}}}}')

attachmentsChatMessageAttachment1.setName(null)

attachmentsChatMessageAttachment1.setThumbnailUrl(null)


attachmentsArray []= attachmentsChatMessageAttachment1;
request_body.setAttachments(attachmentsArray)


hostedContentsChatMessageHostedContent1 = ChatMessageHostedContent()
hostedContentsChatMessageHostedContent1.setContentBytes(base64_decode('iVBORw0KGgoAAAANSUhEUgAABWMAAAEMCAYAAAChuaTsAAAAAXNSR0IArs4'))

hostedContentsChatMessageHostedContent1.setContentType('image/png')

additionalData = [
'@microsoft.graph.temporaryId' => '1', 
];
hostedContentsChatMessageHostedContent1.setAdditionalData(additionalData)



hostedContentsArray []= hostedContentsChatMessageHostedContent1;
hostedContentsChatMessageHostedContent2 = ChatMessageHostedContent()
hostedContentsChatMessageHostedContent2.setContentBytes(base64_decode('iVBORw0KGgoAAAANSUhEUgAAA5YAAAB4CAYAAACJrW0RAAAAAXNSR0IArs4'))

hostedContentsChatMessageHostedContent2.setContentType('image/png')

additionalData = [
'@microsoft.graph.temporaryId' => '2', 
];
hostedContentsChatMessageHostedContent2.setAdditionalData(additionalData)



hostedContentsArray []= hostedContentsChatMessageHostedContent2;
request_body.setHostedContents(hostedContentsArray)




result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body)


```