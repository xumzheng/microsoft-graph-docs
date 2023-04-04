---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ItemAddress();
request_body.setAllowedAudiences(AllowedAudiences('me'));

request_body.setDisplayName('Secret Hideout');



result = await client.usersById('user-id').profile.addressesById('itemAddress-id').patch(request_body);


```