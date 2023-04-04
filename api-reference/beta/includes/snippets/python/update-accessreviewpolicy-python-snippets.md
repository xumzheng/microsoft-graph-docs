---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = AccessReviewPolicy();
request_body.setIsGroupOwnerManagementEnabled(true);



result = await client.policies.accessReviewPolicy.patch(request_body);


```