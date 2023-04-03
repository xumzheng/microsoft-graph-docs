---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CalendarPermission();
requestBody.setRole(CalendarRoleType('write'));



result = awaitclient.usersById('user-id').calendarsById('calendar-id').calendarPermissionsById('calendarPermission-id').patch(requestBody);


```