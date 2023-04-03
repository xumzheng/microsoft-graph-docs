---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UserSource();
requestBody.setEmail('adelev@contoso.com');

requestBody.setIncludedSources(SourceType('mailbox'));



result = awaitclient.compliance().ediscovery().casesById('case-id').legalHoldsById('legalHold-id').userSources().post(requestBody);


```