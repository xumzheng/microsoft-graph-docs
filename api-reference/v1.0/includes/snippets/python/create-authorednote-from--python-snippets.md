---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AuthoredNote();
content = ItemBody();
content.setContent('String');

content.setContentType(BodyType('text'));


requestBody.setContent($content);


result = awaitclient.privacy().subjectRightsRequestsById('subjectRightsRequest-id').notes().post(requestBody);


```