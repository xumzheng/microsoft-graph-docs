---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = LegalHold();
requestBody.setDescription('This is a description for a legalHold');



result = awaitclient.compliance().ediscovery().casesById('case-id').legalHoldsById('legalHold-id').patch(requestBody);


```