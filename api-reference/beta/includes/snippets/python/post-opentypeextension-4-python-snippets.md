---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReplyPostRequestBody()
post = Post()
postBody = ItemBody()
postBody.ContentType(BodyType('html'))

postBody.content = '<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>'


post.body = postBody
extensionsExtension1 = Extension()
extensionsExtension1.@odatatype = 'microsoft.graph.openTypeExtension'

additionalData = [
'extensionName' => 'Com.Contoso.HR', 
'companyName' => 'Contoso', 
'expirationDate' => '2015-07-03T13:04:00.000Z', 
'topPicks' => ['Employees only', 'Add spouse or guest', 'Add family', ],
];
extensionsExtension1.additionaldata(additionalData)



extensionsArray []= extensionsExtension1;
post.extensions(extensionsArray)



request_body.post = post



await client.groups_by_id('group-id').threads_by_id('conversationThread-id').posts_by_id('post-id').reply.post(request_body = request_body)


```