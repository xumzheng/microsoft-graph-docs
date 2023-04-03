---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Calendar();
requestBody.setName('Marketing calendar');



result = await client.me().calendarGroupsById('calendarGroup-id').calendars().post(requestBody);


```