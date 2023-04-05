---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthoredNote()
content = ItemBody()
content.setContent('String')

content.setContentType(BodyType('text'))


request_body.setContent($content)


result = await client.privacy.subjectRightsRequestsby_id('subjectRightsRequest-id').notes.post(request_body)


```