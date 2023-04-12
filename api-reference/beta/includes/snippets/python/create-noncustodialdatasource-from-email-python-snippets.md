---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = NoncustodialDataSource()
request_body.applyHoldToSource = true

dataSource = DataSource()
dataSource.@odatatype = 'microsoft.graph.ediscovery.userSource'

additionalData = [
'email' => 'adelev@contoso.com', 
];
dataSource.additionaldata(additionalData)



request_body.dataSource = dataSource



result = await client.compliance.ediscovery.cases_by_id('case-id').noncustodialDataSources.post(request_body = request_body)


```