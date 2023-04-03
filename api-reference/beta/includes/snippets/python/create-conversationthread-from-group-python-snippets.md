---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ConversationThread();
requestBody.setTopic('New Conversation Thread Topic');

postsPost1 = Post();
postsPost1Body = ItemBody();
postsPost1Body.setContentType(BodyType('html'));

postsPost1Body.setContent('this is body content');


postsPost1.setBody($postsPost1Body);
newParticipantsRecipient1 = Recipient();
newParticipantsRecipient1EmailAddress = EmailAddress();
newParticipantsRecipient1EmailAddress.setName('Alex Darrow');

newParticipantsRecipient1EmailAddress.setAddress('alexd@contoso.com');


newParticipantsRecipient1.setEmailAddress($newParticipantsRecipient1EmailAddress);

newParticipantsArray []= newParticipantsRecipient1;
postsPost1.setNewParticipants(newParticipantsArray);



postsArray []= postsPost1;
requestBody.setPosts(postsArray);




result = awaitclient.groupsById('group-id').threads().post(requestBody);


```