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

postBody.content = 'content-value'


post.body = postBody
post.receivedDateTime = DateTime('datetime-value')

post.has_attachments = True

post_from = Recipient()
post_from_email_address = EmailAddress()
postFromEmailAddress.name = 'name-value'

postFromEmailAddress.address = 'address-value'


postFrom.email_address = postFromEmailAddress

post.from = postFrom
post_sender = Recipient()
post_sender_email_address = EmailAddress()
postSenderEmailAddress.name = 'name-value'

postSenderEmailAddress.address = 'address-value'


postSender.email_address = postSenderEmailAddress

post.sender = postSender
post.conversationThreadId = 'conversationThreadId-value'

new_participants_recipient1 = Recipient()
new_participants_recipient1_email_address = EmailAddress()
newParticipantsRecipient1EmailAddress.name = 'name-value'

newParticipantsRecipient1EmailAddress.address = 'address-value'


newParticipantsRecipient1.email_address = newParticipantsRecipient1EmailAddress

newParticipantsArray []= newParticipantsRecipient1;
post.newparticipants(newParticipantsArray)


post.conversationId = 'conversationId-value'

post.createdDateTime = DateTime('datetime-value')

post.lastModifiedDateTime = DateTime('datetime-value')

post.changeKey = 'changeKey-value'

post.Categories(['categories-value', ])

post.id = 'id-value'

post_in_reply_to = Post()

post.in_reply_to = postInReplyTo
attachments_attachment1 = Attachment()
attachmentsAttachment1.@odatatype = '#microsoft.graph.fileAttachment'

attachmentsAttachment1.lastModifiedDateTime = DateTime('datetime-value')

attachmentsAttachment1.name = 'name-value'

attachmentsAttachment1.contentType = 'contentType-value'

attachmentsAttachment1.size = 99

attachmentsAttachment1.is_inline = True

attachmentsAttachment1.id = 'id-value'


attachmentsArray []= attachmentsAttachment1;
post.attachments(attachmentsArray)



request_body.post = post



await client.groups_by_id('group-id').threads_by_id('conversationThread-id').posts_by_id('post-id').reply.post(request_body = request_body)


```