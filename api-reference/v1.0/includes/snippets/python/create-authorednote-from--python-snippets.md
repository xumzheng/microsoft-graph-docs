---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthoredNote()
content = ItemBody()
content.content = 'String'

content.ContentType(BodyType('text'))


request_body.content = content


request_configuration = NotesRequestBuilderPostRequestConfiguration(
)


result = await client.privacy.subjectRightsRequests_by_id('subjectRightsRequest-id').notes.post(request_body = request_body)


```