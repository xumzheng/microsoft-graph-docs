---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ExternalIdentitiesPolicy();
requestBody.setAllowExternalIdentitiesToLeave(false);



result = await client.policies().externalIdentitiesPolicy().patch(requestBody);


```