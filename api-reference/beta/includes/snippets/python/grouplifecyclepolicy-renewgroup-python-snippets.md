---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = RenewGroupPostRequestBody();
requestBody.setGroupId('ffffffff-ffff-ffff-ffff-ffffffffffff');



result = await client.groupLifecyclePolicies().renewGroup().post(requestBody);


```