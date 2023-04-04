---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = ItemPhone();
request_body.setType(PhoneType('other'));



result = await client.usersById('user-id').profile.phonesById('itemPhone-id').patch(request_body);


```