---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CalendarGroup();
requestBody.setName('name-value');



requestResult = graphServiceClient.me().calendarGroupsById('calendarGroup-id').patch(requestBody);


```