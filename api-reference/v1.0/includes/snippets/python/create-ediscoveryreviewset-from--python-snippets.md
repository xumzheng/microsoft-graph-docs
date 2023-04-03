---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EdiscoveryReviewSet();
requestBody.setDisplayName('My review set 2');



result = await client.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSets().post(requestBody);


```