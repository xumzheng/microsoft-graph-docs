---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = GetMemberObjectsPostRequestBody();
requestBody.setSecurityEnabledOnly(true);



result = await client.directoryObjectsById('directoryObject-id').getMemberObjects().post(requestBody);


```