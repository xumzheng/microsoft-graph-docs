---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EdiscoveryReviewSetQuery();
requestBody.setDisplayName('My Query 1');

requestBody.setContentQuery('(Author=\"edison\")');



result = await client.security().cases().ediscoveryCasesById('ediscoveryCase-id').reviewSetsById('ediscoveryReviewSet-id').queries().post(requestBody);


```