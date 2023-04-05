---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChatMessage()
request_body.setCreatedDateTime(DateTime('2019-02-04T19:58:15.511Z'))

from = ChatMessageFromIdentitySet()
fromUser = Identity()
fromUser.setId('id-value')

fromUser.setDisplayName('Joh Doe')

additionalData = [
'userIdentityType' => 'aadUser', 
];
fromUser.setAdditionalData(additionalData)



from.setUser($fromUser)

request_body.setFrom($from)
body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('Hello World')


request_body.setBody($body)


result = await client.teamsby_id('team-id')_channelsby_id('channel-id')_messages.post(request_body)


```