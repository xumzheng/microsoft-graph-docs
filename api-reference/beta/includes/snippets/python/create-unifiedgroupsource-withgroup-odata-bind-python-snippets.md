---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = UnifiedGroupSource()
request_body.IncludedSources(SourceType('mailbox'))

additionalData = [
'group@odata.bind' => 'https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610', 
];
request_body.additionaldata(additionalData)




request_configuration = UnifiedGroupSourcesRequestBuilderPostRequestConfiguration(
)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').custodians_by_id('ediscoveryCustodian-id').unifiedGroupSources.post(request_body = request_body)


```