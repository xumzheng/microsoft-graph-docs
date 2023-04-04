---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Conversation();
request_body.setTopic('Does anyone have a second?');

threadsConversationThread1 = ConversationThread();
postsPost1 = Post();
postsPost1Body = ItemBody();
postsPost1Body.setContentType(BodyType('html'));

postsPost1Body.setContent('This is urgent!');


postsPost1.setBody($postsPost1Body);
extensionsExtension1 = Extension();
extensionsExtension1.set@odatatype('microsoft.graph.openTypeExtension');

additionalData = [
'extensionName' => 'Com.Contoso.Benefits', 
'companyName' => 'Contoso', 
'expirationDate' => '2016-08-03T11:00:00.000Z', 
'topPicks' => ['Employees only', 'Add spouse or guest', 'Add family', ],
];
extensionsExtension1.setAdditionalData(additionalData);



extensionsArray []= extensionsExtension1;
postsPost1.setExtensions(extensionsArray);



postsArray []= postsPost1;
threadsConversationThread1.setPosts(postsArray);



threadsArray []= threadsConversationThread1;
request_body.setThreads(threadsArray);




result = await client.groupsById('group-id').conversations().post(request_body);


```