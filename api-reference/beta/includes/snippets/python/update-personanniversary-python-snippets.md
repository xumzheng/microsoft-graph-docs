---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PersonAnnualEvent();
requestBody.setAllowedAudiences(AllowedAudiences('contacts'));



result = awaitclient.me().profile().anniversariesById('personAnnualEvent-id').patch(requestBody);


```