---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Conversation()
request_body.topic = 'Does anyone have a second?'

threads_conversation_thread1 = ConversationThread()
posts_post1 = Post()
posts_post1_body = ItemBody()
postsPost1Body.ContentType(BodyType('html'))

postsPost1Body.content = 'This is urgent!'


postsPost1.body = postsPost1Body
extensions_extension1 = Extension()
extensionsExtension1.@odatatype = 'microsoft.graph.openTypeExtension'

additionalData = [
'extensionName' => 'Com.Contoso.Benefits', 
'companyName' => 'Contoso', 
'expirationDate' => '2016-08-03T11:00:00.000Z', 
'topPicks' => ['Employees only', 'Add spouse or guest', 'Add family', ],
];
extensionsExtension1.additionaldata(additionalData)



extensionsArray []= extensionsExtension1;
postsPost1.extensions(extensionsArray)



postsArray []= postsPost1;
threadsConversationThread1.posts(postsArray)



threadsArray []= threadsConversationThread1;
request_body.threads(threadsArray)





result = await client.groups_by_id('group-id').conversations.post(request_body = request_body)


```