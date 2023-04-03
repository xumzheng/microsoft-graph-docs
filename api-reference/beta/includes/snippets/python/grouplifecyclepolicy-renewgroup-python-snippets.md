---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = RenewGroupPostRequestBody();
requestBody.setGroupId('ffffffff-ffff-ffff-ffff-ffffffffffff');



requestResult = graphServiceClient.groupLifecyclePolicies().renewGroup().post(requestBody);


```