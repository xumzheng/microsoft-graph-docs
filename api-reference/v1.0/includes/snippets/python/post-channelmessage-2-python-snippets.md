---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.createdDateTime = DateTime('2019-02-04T19:58:15.511Z')

from = ChatMessageFromIdentitySet()
fromUser = Identity()
fromUser.id = 'id-value'

fromUser.displayName = 'Joh Doe'

additionalData = [
'userIdentityType' => 'aadUser', 
];
fromUser.additionaldata(additionalData)



from.user = fromUser

request_body.from = from
body = ItemBody()
body.ContentType(BodyType('html'))

body.content = 'Hello World'


request_body.body = body



result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body = request_body)


```