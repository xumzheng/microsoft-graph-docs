---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = TemporaryAccessPassAuthenticationMethod();
requestBody.setStartDateTime(DateTime('2022-06-05T00:00:00.000Z'));

requestBody.setLifetimeInMinutes(60);

requestBody.setIsUsableOnce(false);



result = await client.usersById('user-id').authentication().temporaryAccessPassMethods().post(requestBody);


```