---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Calendar();
requestBody.setName('Marketing calendar');



requestResult = graphServiceClient.me().calendarGroupsById('calendarGroup-id').calendars().post(requestBody);


```