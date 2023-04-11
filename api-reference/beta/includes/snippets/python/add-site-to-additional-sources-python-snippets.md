---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DataSource()
request_body.@odatatype = 'microsoft.graph.ediscovery.siteSource'

additionalData = [
'site' => request_body = Site()
		request_body.webUrl = 'https://contoso.sharepoint.com/sites/SecretSite'


request_body.site = site

];
request_body.additionaldata(additionalData)




request_configuration = AdditionalSourcesRequestBuilderPostRequestConfiguration(
)


result = await client.compliance.ediscovery.cases_by_id('case-id').sourceCollections_by_id('sourceCollection-id').additionalSources.post(request_body = request_body)


```