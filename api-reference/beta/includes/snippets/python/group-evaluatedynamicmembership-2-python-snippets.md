---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EvaluateDynamicMembershipPostRequestBody();
requestBody.setMemberId('319b41e8-d9e4-42f8-bdc9-741113f48b33');

requestBody.setMembershipRule('(user.displayName -startsWith \"EndTestUser\")');



result = awaitclient.groups().evaluateDynamicMembership().post(requestBody);


```