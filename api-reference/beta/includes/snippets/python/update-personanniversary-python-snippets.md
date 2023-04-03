---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = PersonAnnualEvent();
requestBody.setAllowedAudiences(AllowedAudiences('contacts'));



result = await client.me().profile().anniversariesById('personAnnualEvent-id').patch(requestBody);


```