---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = RenewGroupPostRequestBody();
request_body.setGroupId('ffffffff-ffff-ffff-ffff-ffffffffffff');



result = await client.groupLifecyclePolicies().renewGroup().post(request_body);


```