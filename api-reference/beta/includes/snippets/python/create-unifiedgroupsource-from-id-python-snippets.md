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




result = await client.compliance_ediscovery_casesby_id('case-id')_custodiansby_id('custodian-id')_unifiedGroupSources.post(request_body)


```