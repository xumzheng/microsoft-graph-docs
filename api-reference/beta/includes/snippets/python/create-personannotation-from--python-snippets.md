---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PersonAnnotation();
detail = ItemBody();
detail.setContentType(BodyType('text'));

detail.setContent('I am originally from Australia, but grew up in Moscow, Russia.');


requestBody.setDetail($detail);
requestBody.setDisplayName('About Me');



result = awaitclient.me().profile().notes().post(requestBody);


```