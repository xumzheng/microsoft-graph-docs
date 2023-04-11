---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalendarPermission()
request_body.Role(CalendarRoleType('write'))




result = await client.users_by_id('user-id').calendar.calendarPermissions_by_id('calendarPermission-id').patch(request_body = request_body)


```