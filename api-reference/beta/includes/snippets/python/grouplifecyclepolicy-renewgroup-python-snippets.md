---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = RenewGroupPostRequestBody();
requestBody.setGroupId('ffffffff-ffff-ffff-ffff-ffffffffffff');



result = awaitclient.groupLifecyclePolicies().renewGroup().post(requestBody);


```