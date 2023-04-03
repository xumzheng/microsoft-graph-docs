---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CalendarPermission();
requestBody.setRole(CalendarRoleType('write'));



result = await client.usersById('user-id').calendarsById('calendar-id').calendarPermissionsById('calendarPermission-id').patch(requestBody);


```