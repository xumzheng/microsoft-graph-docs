---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DataSource()
request_body.set@odatatype('microsoft.graph.ediscovery.siteSource')

additionalData = [
'site' => request_body = Site()
		request_body.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite')


request_body.setSite($site)

];
request_body.setAdditionalData(additionalData)



request_config = AdditionalSourcesRequestBuilderPostRequestConfiguration(
request_config = AdditionalSourcesRequestBuilderPostRequestConfiguration(query_params=)


result = await client.compliance.ediscovery.cases_by_id('case-id').sourceCollections_by_id('sourceCollection-id').additionalSources.post(request_body, headers=)


```