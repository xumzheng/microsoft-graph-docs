---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UserSource();
requestBody.setEmail('adelev@contoso.com');

requestBody.setIncludedSources(SourceType('mailbox'));



requestResult = graphServiceClient.compliance().ediscovery().casesById('case-id').legalHoldsById('legalHold-id').userSources().post(requestBody);


```