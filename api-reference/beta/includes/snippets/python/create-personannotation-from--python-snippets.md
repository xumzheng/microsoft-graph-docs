---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = PersonAnnotation();
detail = ItemBody();
detail.setContentType(BodyType('text'));

detail.setContent('I am originally from Australia, but grew up in Moscow, Russia.');


request_body.setDetail($detail);
request_body.setDisplayName('About Me');



result = await client.me.profile.notes.post(request_body);


```