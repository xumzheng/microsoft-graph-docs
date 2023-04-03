---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = GetMemberObjectsPostRequestBody();
requestBody.setSecurityEnabledOnly(true);



requestResult = graphServiceClient.me().getMemberObjects().post(requestBody);


```