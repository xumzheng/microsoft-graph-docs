---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalendarPermission()
request_body.setRole(CalendarRoleType('write'))



result = await client.usersby_id('user-id').calendarsby_id('calendar-id').calendarPermissionsby_id('calendarPermission-id').patch(request_body)


```