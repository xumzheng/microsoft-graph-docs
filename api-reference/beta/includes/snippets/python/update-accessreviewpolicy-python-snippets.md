---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AccessReviewPolicy();
requestBody.setIsGroupOwnerManagementEnabled(true);



requestResult = graphServiceClient.policies().accessReviewPolicy().patch(requestBody);


```