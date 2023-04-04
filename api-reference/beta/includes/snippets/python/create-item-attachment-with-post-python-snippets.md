---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ReplyPostRequestBody()
post = Post()
postBody = ItemBody()
postBody.setContentType(BodyType('text'))

postBody.setContent('I attached an event.')


post.setBody($postBody)
attachmentsAttachment1 = Attachment()
attachmentsAttachment1.set@odatatype('#microsoft.graph.itemAttachment')

attachmentsAttachment1.setName('Holiday event')

additionalData = [
'item' => attachmentsAttachment1 = Item()
		attachmentsAttachment1.set@odatatype('microsoft.graph.event')

		attachmentsAttachment1.setSubject('Discuss gifts for children')

body = Body()
		body.setContentType('HTML')

		body.setContent('Let\'s look for funding!')


attachmentsAttachment1.setBody($body)
start = Start()
		start.setDateTime('2019-12-02T18:00:00')

		start.setTimeZone('Pacific Standard Time')


attachmentsAttachment1.setStart($start)
end = End()
		end.setDateTime('2019-12-02T19:00:00')

		end.setTimeZone('Pacific Standard Time')


attachmentsAttachment1.setEnd($end)

attachmentsAttachment1.setItem($item)

];
attachmentsAttachment1.setAdditionalData(additionalData)



attachmentsArray []= attachmentsAttachment1;
post.setAttachments(attachmentsArray)



request_body.setPost($post)


await client.groupsById('group-id').threadsById('conversationThread-id').reply.post(request_body)


```