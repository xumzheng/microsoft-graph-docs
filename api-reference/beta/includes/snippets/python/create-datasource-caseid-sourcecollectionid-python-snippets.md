---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DataSource()
request_body.@odatatype = 'microsoft.graph.ediscovery.userSource'

additionalData = [
'email' => 'badguy@contoso.com', 
];
request_body.additionaldata(additionalData)





result = await client.compliance.ediscovery.cases_by_id('case-id').sourceCollections_by_id('sourceCollection-id').additionalSources.post(request_body = request_body)


```