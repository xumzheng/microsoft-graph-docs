---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = UnifiedGroupSource();
requestBody.setIncludedSources(SourceType('mailbox'));

additionalData = [
'group@odata.bind' => 'https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.security().cases().ediscoveryCasesById('ediscoveryCase-id').custodiansById('ediscoveryCustodian-id').unifiedGroupSources().post(requestBody);


```