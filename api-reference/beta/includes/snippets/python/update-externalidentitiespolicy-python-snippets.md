---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ExternalIdentitiesPolicy();
requestBody.setAllowExternalIdentitiesToLeave(false);



requestResult = graphServiceClient.policies().externalIdentitiesPolicy().patch(requestBody);


```