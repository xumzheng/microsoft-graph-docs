---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryNoncustodialDataSource()
dataSource = DataSource()
dataSource.@odatatype = 'microsoft.graph.security.siteSource'

additionalData = [
'site' => dataSource = Site()
		dataSource.webUrl = 'https://m365x809305.sharepoint.com/sites/Design-topsecret'


dataSource.site = site

];
dataSource.additionaldata(additionalData)



request_body.dataSource = dataSource



result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').noncustodialDataSources.post(request_body = request_body)


```