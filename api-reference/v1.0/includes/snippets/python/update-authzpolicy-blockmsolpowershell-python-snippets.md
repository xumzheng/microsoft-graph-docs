---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AuthorizationPolicy();
requestBody.setBlockMsolPowerShell(true);



result = awaitclient.policies().authorizationPolicy().patch(requestBody);


```