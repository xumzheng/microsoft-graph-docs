---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UserSource();
requestBody.setEmail('megan@contoso.com');

requestBody.setIncludedSources(SourceType('mailbox, site'));



result = awaitclient.compliance().ediscovery().casesById('case-id').custodiansById('custodian-id').userSources().post(requestBody);


```