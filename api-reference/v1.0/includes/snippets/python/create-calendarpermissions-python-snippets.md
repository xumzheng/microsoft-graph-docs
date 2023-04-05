---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CalendarPermission()
emailAddress = EmailAddress()
emailAddress.setName('Samantha Booth')

emailAddress.setAddress('samanthab@adatum.onmicrosoft.com')


request_body.setEmailAddress($emailAddress)
request_body.setIsInsideOrganization(true)

request_body.setIsRemovable(true)

request_body.setRole(CalendarRoleType('read'))



result = await client.me.calendar.calendarPermissions.post(request_body)


```