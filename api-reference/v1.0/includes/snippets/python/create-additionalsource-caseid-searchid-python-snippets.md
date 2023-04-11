---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DataSource()
request_body.@odatatype = 'microsoft.graph.security.siteSource'

additionalData = [
'site' => request_body = Site()
		request_body.webUrl = 'https://contoso.sharepoint.com/sites/SecretSite'


request_body.site = site

];
request_body.additionaldata(additionalData)




request_configuration = AdditionalSourcesRequestBuilderPostRequestConfiguration(
)


result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').searches_by_id('ediscoverySearch-id').additionalSources.post(request_body = request_body)


```