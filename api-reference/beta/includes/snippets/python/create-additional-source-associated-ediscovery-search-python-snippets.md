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
		request_body.setWebUrl('https://m365x809305.sharepoint.com/sites/Design-topsecret')


request_body.setSite($site)

];
request_body.setAdditionalData(additionalData)




result = await client.security_cases_ediscoveryCasesby_id('ediscoveryCase-id')_searchesby_id('ediscoverySearch-id')_additionalSources.post(request_body)


```