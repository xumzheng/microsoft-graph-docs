---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Case();
requestBody.setDisplayName('My Case 1');



result = await client.compliance().ediscovery().cases().post(requestBody);


```