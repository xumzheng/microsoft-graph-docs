---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = PersonAnnualEvent();
requestBody.setAllowedAudiences(AllowedAudiences('contacts'));



requestResult = graphServiceClient.me().profile().anniversariesById('personAnnualEvent-id').patch(requestBody);


```