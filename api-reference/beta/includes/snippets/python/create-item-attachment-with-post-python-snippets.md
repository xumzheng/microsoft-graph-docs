---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReplyPostRequestBody()
post = Post()
post_body = ItemBody()
postBody.ContentType(BodyType('text'))

postBody.content = 'I attached an event.'


post.body = postBody
attachments_attachment1 = Attachment()
attachmentsAttachment1.@odatatype = '#microsoft.graph.itemAttachment'

attachmentsAttachment1.name = 'Holiday event'

additionalData = [
'item' => attachments_attachment1 = Item()
		attachmentsAttachment1.@odatatype = 'microsoft.graph.event'

		attachmentsAttachment1.subject = 'Discuss gifts for children'

body = Body()
		body.contentType = 'HTML'

		body.content = 'Let\'s look for funding!'


attachmentsAttachment1.body = body
start = Start()
		start.dateTime = '2019-12-02T18:00:00'

		start.timeZone = 'Pacific Standard Time'


attachmentsAttachment1.start = start
end = End()
		end.dateTime = '2019-12-02T19:00:00'

		end.timeZone = 'Pacific Standard Time'


attachmentsAttachment1.end = end

attachmentsAttachment1.item = item

];
attachmentsAttachment1.additionaldata(additionalData)



attachmentsArray []= attachmentsAttachment1;
post.attachments(attachmentsArray)



request_body.post = post



await client.groups_by_id('group-id').threads_by_id('conversationThread-id').reply.post(request_body = request_body)


```