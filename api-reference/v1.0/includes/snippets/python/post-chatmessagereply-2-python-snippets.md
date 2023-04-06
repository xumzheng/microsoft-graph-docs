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
fromUser.setId('8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca')

fromUser.setDisplayName('John Doe')


from.setUser($fromUser)

request_body.setFrom($from)
body = ItemBody()
body.setContentType(BodyType('html'))

body.setContent('Hello World')


request_body.setBody($body)

request_config = RepliesRequestBuilderPostRequestConfiguration(
request_config = RepliesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages_by_id('chatMessage-id').replies.post(request_body, headers=)


```