---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AuthorizationPolicy();
requestBody.setAllowEmailVerifiedUsersToJoinOrganization(false);



result = await client.policies().authorizationPolicy().patch(requestBody);


```