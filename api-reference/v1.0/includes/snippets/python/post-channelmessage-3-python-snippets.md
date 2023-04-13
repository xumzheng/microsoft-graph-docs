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

fromUser.displayName = 'John Doe'

additionalData = [
'userIdentityType' => 'aadUser', 
];
fromUser.additionaldata(additionalData)



from.user = fromUser

request_body.from = from
body = ItemBody()
body.ContentType(BodyType('html'))

body.content = '<div><div>\n<div><span><img height=\"250\" src=\"../hostedContents/1/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>'


request_body.body = body
hostedContentsChatMessageHostedContent1 = ChatMessageHostedContent()
hostedContentsChatMessageHostedContent1.ContentBytes(base64_decode('iVBORw0KGgoAAAANSUhEUgAAANcAAAExCAYAAADvFzeeAAAXjklEQVR4Ae2d/XNU1RnH+9e0FFrA0RCIyaS8hRA0HV5KbS1gHRgVpjMClY4GHJ3yYm1HCmXaWttaaZUZtIIFKYi8lFAkvOQ9u5vN225IARVBbX9/Os9NbrLZbMjmhCfJPX5+2Lmb3T25y3O+n/M599x7w9f+++UXwoMakIF7n4GvUdR7X1RqSk01A8CFuZm5GGUAuIwKi72wF3ABF+YyygBwGRUWc2Eu4AIuzGWUAeAyKizmwlzABVyYyygDwGVUWMyFuYALuDCXUQaAy6iwmAtzARdwfWXMdeuzT+TGxz3Sfb1LunrapL07IW3pePDQ5/qavqef0c+OdYAELuAac4jGGkLL9rdvfyo9N9ODQAqBGmmrwGlb/R0u3xG4gMspOC5hG882CoRaaCSA8n1ff9doIQMu4PIOrus3u+8ZVNnw6e/Od5AALuDKOyz5hmqiPnfnzi1J9bSbgRWCpvvQfY307wQu4BoxJCOFaDK8rwsQmQsUIQhWW93XSIsewAVckYdLQ24F0Ui/926AARdwRRounZ6Np7GyYdN9DzdFBC7gijRc43GMlQ1U9s/6HXJNjYELuHI<<-----Removed----->>>>'))

hostedContentsChatMessageHostedContent1.contentType = 'image/png'

additionalData = [
'@microsoft.graph.temporaryId' => '1', 
];
hostedContentsChatMessageHostedContent1.additionaldata(additionalData)



hostedContentsArray []= hostedContentsChatMessageHostedContent1;
request_body.hostedcontents(hostedContentsArray)





result = await client.teams_by_id('team-id').channels_by_id('channel-id').messages.post(request_body = request_body)


```