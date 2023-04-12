---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalendarPermission()
emailAddress = EmailAddress()
emailAddress.name = 'Samantha Booth'

emailAddress.address = 'samanthab@adatum.onmicrosoft.com'


request_body.emailAddress = emailAddress
request_body.isInsideOrganization = true

request_body.isRemovable = true

request_body.Role(CalendarRoleType('read'))




result = await client.users_by_id('user-id').calendar.calendarPermissions.post(request_body = request_body)


```