---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NoncustodialDataSource()
request_body.setApplyHoldToSource(false)

dataSource = DataSource()
dataSource.set@odatatype('microsoft.graph.ediscovery.siteSource')

additionalData = [
'site' => dataSource = Site()
		dataSource.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite')


dataSource.setSite($site)

];
dataSource.setAdditionalData(additionalData)



request_body.setDataSource($dataSource)


result = await client.compliance.ediscovery.cases_by_id('case-id').noncustodialDataSources.post(request_body)


```