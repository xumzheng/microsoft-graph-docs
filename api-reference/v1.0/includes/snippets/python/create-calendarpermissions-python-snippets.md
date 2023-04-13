---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalendarPermission()
email_address = EmailAddress()
emailAddress.name = 'Samantha Booth'

emailAddress.address = 'samanthab@adatum.onmicrosoft.com'


request_body.email_address = emailAddress
request_body.is_inside_organization = True

request_body.is_removable = True

request_body.Role(CalendarRoleType('read'))




result = await client.me.calendar.calendarPermissions.post(request_body = request_body)


```