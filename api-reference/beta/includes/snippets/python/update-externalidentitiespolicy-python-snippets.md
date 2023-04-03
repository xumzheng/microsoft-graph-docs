---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ExternalIdentitiesPolicy();
requestBody.setAllowExternalIdentitiesToLeave(false);



result = awaitclient.policies().externalIdentitiesPolicy().patch(requestBody);


```