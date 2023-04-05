---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DataSource()
request_body.set@odatatype('microsoft.graph.security.siteSource')

additionalData = [
'site' => request_body = Site()
		request_body.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite')


request_body.setSite($site)

];
request_body.setAdditionalData(additionalData)




result = await client.security.cases.ediscoveryCases._by_id('ediscoveryCase-id').searches._by_id('ediscoverySearch-id').additionalSources.post(request_body)


```