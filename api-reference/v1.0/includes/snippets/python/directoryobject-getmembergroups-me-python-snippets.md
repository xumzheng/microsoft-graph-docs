---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = GetMemberGroupsPostRequestBody();
request_body.setSecurityEnabledOnly(true);



result = await client.me().getMemberGroups().post(request_body);


```