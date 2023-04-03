---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ReplyPostRequestBody();
post = Post();
postBody = ItemBody();
postBody.setContentType(BodyType('html'));

postBody.setContent('<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>');


post.setBody($postBody);
extensionsExtension1 = Extension();
extensionsExtension1.set@odatatype('microsoft.graph.openTypeExtension');

additionalData = [
'extensionName' => 'Com.Contoso.HR', 
'companyName' => 'Contoso', 
'expirationDate' => '2015-07-03T13:04:00.000Z', 
'topPicks' => ['Employees only', 'Add spouse or guest', 'Add family', ],
];
extensionsExtension1.setAdditionalData(additionalData);



extensionsArray []= extensionsExtension1;
post.setExtensions(extensionsArray);



requestBody.setPost($post);


await client.groupsById('group-id').threadsById('conversationThread-id').postsById('post-id').reply().post(requestBody);


```