---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = GetMemberObjectsPostRequestBody();
request_body.setSecurityEnabledOnly(true);



result = await client.directoryObjectsById('directoryObject-id').getMemberObjects.post(request_body);


```