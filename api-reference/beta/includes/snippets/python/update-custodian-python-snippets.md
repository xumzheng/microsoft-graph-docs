---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Custodian();
requestBody.setApplyHoldToSources(false);



result = awaitclient.compliance().ediscovery().casesById('case-id').custodiansById('custodian-id').patch(requestBody);


```