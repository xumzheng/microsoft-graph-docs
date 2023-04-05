---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DataSource()
request_body.set@odatatype('microsoft.graph.ediscovery.userSource')

additionalData = [
'email' => 'badguy@contoso.com', 
];
request_body.setAdditionalData(additionalData)




result = await client.compliance_ediscovery_casesby_id('case-id')_sourceCollectionsby_id('sourceCollection-id')_additionalSources.post(request_body)


```