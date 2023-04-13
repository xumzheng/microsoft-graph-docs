---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Conversation()
request_body.topic = 'Take your wellness days and rest'

threads_conversation_thread1 = ConversationThread()
posts_post1 = Post()
posts_post1_body = ItemBody()
postsPost1Body.ContentType(BodyType('html'))

postsPost1Body.content = 'Contoso cares about you: Rest and Recharge'


postsPost1.body = postsPost1Body
new_participants_recipient1 = Recipient()
new_participants_recipient1_email_address = EmailAddress()
newParticipantsRecipient1EmailAddress.name = 'Adele Vance'

newParticipantsRecipient1EmailAddress.address = 'AdeleV@contoso.onmicrosoft.com'


newParticipantsRecipient1.email_address = newParticipantsRecipient1EmailAddress

newParticipantsArray []= newParticipantsRecipient1;
postsPost1.newparticipants(newParticipantsArray)



postsArray []= postsPost1;
threadsConversationThread1.posts(postsArray)



threadsArray []= threadsConversationThread1;
request_body.threads(threadsArray)





result = await client.groups_by_id('group-id').conversations.post(request_body = request_body)


```