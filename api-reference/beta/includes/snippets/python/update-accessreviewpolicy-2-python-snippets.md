---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = AccessReviewPolicy();
requestBody.setIsGroupOwnerManagementEnabled(true);



result = awaitclient.identityGovernance().accessReviews().policy().patch(requestBody);


```