---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ChatMessage();
requestBody.setMessageType(ChatMessageType('message'));

requestBody.setSubject(null);

requestBody.setSummary(null);

requestBody.setImportance(ChatMessageImportance('normal'));

requestBody.setLocale('en-us');

from = ChatMessageFromIdentitySet();
From.setApplication(null);

From.setDevice(null);

fromUser = Identity();
fromUser.setId('3b102402-813e-4e17-a6b2-f841aef1fdfc');

fromUser.setDisplayName('Sumit Gupta');

additionalData = [
'userIdentityType' => 'aadUser', 
];
fromUser.setAdditionalData(additionalData);



from.setUser($fromUser);
additionalData = [
'conversation' => 		null,
];
from.setAdditionalData(additionalData);



requestBody.setFrom($from);
body = ItemBody();
body.setContentType(BodyType('text'));

body.setContent('Edit text only');


requestBody.setBody($body);
requestBody.setAttachments([]);

requestBody.setMentions([]);

requestBody.setReactions([]);

requestBody.setMessageHistory([]);



result = awaitclient.teamsById('team-id').channelsById('channel-id').messagesById('chatMessage-id').patch(requestBody);


```