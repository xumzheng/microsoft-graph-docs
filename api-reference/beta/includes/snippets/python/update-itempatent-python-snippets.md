---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ItemPatent();
requestBody.setNumber('USPTO-3954432633');

requestBody.setWebUrl('https://patents.gov/3954432633');



result = await client.usersById('user-id').profile().patentsById('itemPatent-id').patch(requestBody);


```