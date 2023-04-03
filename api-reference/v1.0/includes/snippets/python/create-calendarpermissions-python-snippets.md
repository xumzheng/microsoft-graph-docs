---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = CalendarPermission();
emailAddress = EmailAddress();
emailAddress.setName('Samantha Booth');

emailAddress.setAddress('samanthab@adatum.onmicrosoft.com');


requestBody.setEmailAddress($emailAddress);
requestBody.setIsInsideOrganization(true);

requestBody.setIsRemovable(true);

requestBody.setRole(CalendarRoleType('read'));



result = awaitclient.me().calendar().calendarPermissions().post(requestBody);


```