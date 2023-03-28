---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CalendarPermission();
$requestBody.setRole(new CalendarRoleType('write'));



$requestResult = $graphServiceClient.usersById('user-id').calendarsById('calendar-id').calendarPermissionsById('calendarPermission-id').patch($requestBody);


```