---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AuthoredNote()
content = ItemBody()
content.setContent('Please take a look at the files tagged with follow up')

content.setContentType(BodyType('text'))


request_body.setContent($content)


result = await client.privacy_subjectRightsRequestsby_id('subjectRightsRequest-id')_notes.post(request_body)


```