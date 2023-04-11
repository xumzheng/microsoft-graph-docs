---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Conversation()
request_body.topic = 'Take your wellness days and rest'

threadsConversationThread1 = ConversationThread()
postsPost1 = Post()
postsPost1Body = ItemBody()
postsPost1Body.ContentType(BodyType('html'))

postsPost1Body.content = 'Contoso cares about you: Rest and Recharge'


postsPost1.body = postsPost1Body
newParticipantsRecipient1 = Recipient()
newParticipantsRecipient1EmailAddress = EmailAddress()
newParticipantsRecipient1EmailAddress.name = 'Adele Vance'

newParticipantsRecipient1EmailAddress.address = 'AdeleV@contoso.onmicrosoft.com'


newParticipantsRecipient1.emailAddress = newParticipantsRecipient1EmailAddress

newParticipantsArray []= newParticipantsRecipient1;
postsPost1.newparticipants(newParticipantsArray)



postsArray []= postsPost1;
threadsConversationThread1.posts(postsArray)



threadsArray []= threadsConversationThread1;
request_body.threads(threadsArray)




request_configuration = ConversationsRequestBuilderPostRequestConfiguration(
)


result = await client.groups_by_id('group-id').conversations.post(request_body = request_body)


```