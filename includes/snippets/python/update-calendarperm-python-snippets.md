---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalendarPermission()
request_body.setRole(CalendarRoleType('write'))



result = await client.usersById('user-id').calendarsById('calendar-id').calendarPermissionsById('calendarPermission-id').patch(request_body)


```