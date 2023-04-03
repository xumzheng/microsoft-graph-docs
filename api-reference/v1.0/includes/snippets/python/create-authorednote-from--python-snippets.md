---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AuthoredNote();
content = ItemBody();
content.setContent('String');

content.setContentType(BodyType('text'));


requestBody.setContent($content);


requestResult = graphServiceClient.privacy().subjectRightsRequestsById('subjectRightsRequest-id').notes().post(requestBody);


```