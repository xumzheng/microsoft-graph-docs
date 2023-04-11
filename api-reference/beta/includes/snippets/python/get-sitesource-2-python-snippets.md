---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = SiteSourceRequestBuilderGetRequestConfiguration(
)


result = await client.compliance.ediscovery.cases_by_id('case-id').custodians_by_id('custodian-id').siteSources_by_id('siteSource-id').get()


```