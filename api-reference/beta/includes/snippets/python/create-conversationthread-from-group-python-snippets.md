---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConversationThread()
request_body.topic = 'New Conversation Thread Topic'

postsPost1 = Post()
postsPost1Body = ItemBody()
postsPost1Body.ContentType(BodyType('html'))

postsPost1Body.content = 'this is body content'


postsPost1.body = postsPost1Body
newParticipantsRecipient1 = Recipient()
newParticipantsRecipient1EmailAddress = EmailAddress()
newParticipantsRecipient1EmailAddress.name = 'Alex Darrow'

newParticipantsRecipient1EmailAddress.address = 'alexd@contoso.com'


newParticipantsRecipient1.emailAddress = newParticipantsRecipient1EmailAddress

newParticipantsArray []= newParticipantsRecipient1;
postsPost1.newparticipants(newParticipantsArray)



postsArray []= postsPost1;
request_body.posts(postsArray)





result = await client.groups_by_id('group-id').threads.post(request_body = request_body)


```