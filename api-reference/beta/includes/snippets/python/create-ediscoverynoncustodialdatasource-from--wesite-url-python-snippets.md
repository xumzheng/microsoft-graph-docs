---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryNoncustodialDataSource()
data_source = DataSource()
dataSource.@odatatype = 'microsoft.graph.security.siteSource'

additionalData = [
'site' => data_source = Site()
		dataSource.webUrl = 'https://m365x809305.sharepoint.com/sites/Design-topsecret'


dataSource.site = site

];
dataSource.additionaldata(additionalData)



request_body.data_source = dataSource



result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').noncustodialDataSources.post(request_body = request_body)


```