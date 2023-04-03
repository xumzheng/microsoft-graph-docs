---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = EdiscoveryCase();
requestBody.setDisplayName('My Case 1 - Renamed');

requestBody.setDescription('Updated description');



result = awaitclient.security().cases().ediscoveryCasesById('ediscoveryCase-id').patch(requestBody);


```