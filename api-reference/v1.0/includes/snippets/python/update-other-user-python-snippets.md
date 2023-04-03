---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = User();
requestBody.setBusinessPhones(['+1 425 555 0109', ]);

requestBody.setOfficeLocation('18/2111');



result = await client.usersById('user-id').patch(requestBody);


```