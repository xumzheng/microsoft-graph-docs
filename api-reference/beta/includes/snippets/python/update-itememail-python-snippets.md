---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ItemEmail();
requestBody.setDisplayName('Business Email');

requestBody.setType(EmailType('work'));



result = await client.usersById('user-id').profile().emailsById('itemEmail-id').patch(requestBody);


```