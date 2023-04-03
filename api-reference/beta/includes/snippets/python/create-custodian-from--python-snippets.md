---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Custodian();
requestBody.setEmail('AdeleV@contoso.com');

requestBody.setApplyHoldToSources(true);



result = awaitclient.compliance().ediscovery().casesById('case-id').custodians().post(requestBody);


```