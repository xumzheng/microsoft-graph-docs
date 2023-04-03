---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Conversation();
requestBody.setTopic('New head count');

threadsConversationThread1 = ConversationThread();
postsPost1 = Post();
postsPost1Body = ItemBody();
postsPost1Body.setContentType(BodyType('html'));

postsPost1Body.setContent('The confirmation will come by the end of the week.');


postsPost1.setBody($postsPost1Body);
newParticipantsRecipient1 = Recipient();
newParticipantsRecipient1EmailAddress = EmailAddress();
newParticipantsRecipient1EmailAddress.setName('Adele Vance');

newParticipantsRecipient1EmailAddress.setAddress('AdeleV@contoso.onmicrosoft.com');


newParticipantsRecipient1.setEmailAddress($newParticipantsRecipient1EmailAddress);

newParticipantsArray []= newParticipantsRecipient1;
postsPost1.setNewParticipants(newParticipantsArray);



postsArray []= postsPost1;
threadsConversationThread1.setPosts(postsArray);



threadsArray []= threadsConversationThread1;
requestBody.setThreads(threadsArray);




requestResult = graphServiceClient.groupsById('group-id').conversations().post(requestBody);


```