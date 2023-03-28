---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ItemEmail();
$requestBody.setDisplayName('Business Email');

$requestBody.setType(new EmailType('work'));



$requestResult = $graphServiceClient.usersById('user-id').profile().emailsById('itemEmail-id').patch($requestBody);


```