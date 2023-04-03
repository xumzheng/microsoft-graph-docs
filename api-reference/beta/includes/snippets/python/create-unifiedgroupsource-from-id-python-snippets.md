---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = UnifiedGroupSource();
requestBody.setIncludedSources(SourceType('mailbox, site'));

additionalData = [
'group@odata.bind' => 'https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84', 
];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.compliance().ediscovery().casesById('case-id').custodiansById('custodian-id').unifiedGroupSources().post(requestBody);


```