---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ItemAddress();
requestBody.setAllowedAudiences(AllowedAudiences('me'));

requestBody.setDisplayName('Secret Hideout');



result = await client.usersById('user-id').profile().addressesById('itemAddress-id').patch(requestBody);


```