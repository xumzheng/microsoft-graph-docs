---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Case();
requestBody.setDisplayName('My Case 1');



requestResult = graphServiceClient.compliance().ediscovery().cases().post(requestBody);


```