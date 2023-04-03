---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AuthoredNote();
content = ItemBody();
content.setContent('Please take a look at the files tagged with follow up');

content.setContentType(BodyType('text'));


requestBody.setContent($content);


result = await client.privacy().subjectRightsRequestsById('subjectRightsRequest-id').notes().post(requestBody);


```