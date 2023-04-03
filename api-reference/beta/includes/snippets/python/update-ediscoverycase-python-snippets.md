---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = EdiscoveryCase();
requestBody.setDisplayName('My Case 1 - Renamed');

requestBody.setDescription('Updated description');



result = await client.security().cases().ediscoveryCasesById('ediscoveryCase-id').patch(requestBody);


```