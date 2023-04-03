---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ReviewSet();
requestBody.setDisplayName('My Reviewset 3');



result = await client.compliance().ediscovery().casesById('case-id').reviewSets().post(requestBody);


```