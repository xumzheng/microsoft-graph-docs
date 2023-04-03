---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Custodian();
requestBody.setEmail('AdeleV@contoso.com');

requestBody.setApplyHoldToSources(true);



result = await client.compliance().ediscovery().casesById('case-id').custodians().post(requestBody);


```