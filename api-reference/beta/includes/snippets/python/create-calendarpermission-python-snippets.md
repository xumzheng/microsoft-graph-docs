---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new CalendarPermission();
$emailAddress = new EmailAddress();
$emailAddress->setName('Samantha Booth');

$emailAddress->setAddress('samanthab@adatum.onmicrosoft.com');


$requestBody->setEmailAddress($emailAddress);
$requestBody->setIsInsideOrganization(true);

$requestBody->setIsRemovable(true);

$requestBody->setRole(new CalendarRoleType('read'));



$requestResult = $graphServiceClient->usersById('user-id')->calendar()->calendarPermissions()->post($requestBody);


```