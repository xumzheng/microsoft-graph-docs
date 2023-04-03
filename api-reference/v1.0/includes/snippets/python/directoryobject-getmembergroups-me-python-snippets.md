---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = GetMemberGroupsPostRequestBody();
requestBody.setSecurityEnabledOnly(true);



result = await client.me().getMemberGroups().post(requestBody);


```