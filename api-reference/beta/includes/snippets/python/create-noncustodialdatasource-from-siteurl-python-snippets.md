---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NoncustodialDataSource()
request_body.apply_hold_to_source = False

data_source = DataSource()
dataSource.@odatatype = 'microsoft.graph.ediscovery.siteSource'

additionalData = [
'site' => data_source = Site()
		dataSource.webUrl = 'https://contoso.sharepoint.com/sites/SecretSite'


dataSource.site = site

];
dataSource.additionaldata(additionalData)



request_body.data_source = dataSource



result = await client.compliance.ediscovery.cases_by_id('case-id').noncustodialDataSources.post(request_body = request_body)


```