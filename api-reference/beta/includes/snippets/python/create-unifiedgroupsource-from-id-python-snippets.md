---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedGroupSource()
request_body.setIncludedSources(SourceType('mailbox, site'))

additionalData = [
'group@odata.bind' => 'https://graph.microsoft.com/v1.0/groups/b96f95c5-b1b3-4142-b039-8ac79e7d2c84', 
];
request_body.setAdditionalData(additionalData)




result = await client.compliance.ediscovery.casesById('case-id').custodiansById('custodian-id').unifiedGroupSources.post(request_body)


```