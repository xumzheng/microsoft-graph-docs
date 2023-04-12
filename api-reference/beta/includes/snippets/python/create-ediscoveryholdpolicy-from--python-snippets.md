---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EdiscoveryHoldPolicy()
request_body.displayname = 'My legalHold with sources'

request_body.description = 'Created from Graph API'

additionalData = [
'userSources@odata.bind' => userSources@odatabind1 = ()
		userSources@odatabind1.@odatatype = 'microsoft.graph.security.userSource'

		userSources@odatabind1.email = 'SalesTeam@M365x809305.OnMicrosoft.com'


userSources@odata.bindArray []= userSources@odatabind1;
request_body.usersources@odatabind(userSources@odata.bindArray)


'siteSources@odata.bind' => siteSources@odatabind1 = ()
	siteSources@odatabind1.@odatatype = 'microsoft.graph.security.siteSource'

siteSources@odatabind1Site = Site()
	siteSources@odatabind1Site.webUrl = 'https://m365x809305.sharepoint.com/sites/Design-topsecret'


siteSources@odatabind1.site = siteSources@odatabind1Site

siteSources@odata.bindArray []= siteSources@odatabind1;
request_body.sitesources@odatabind(siteSources@odata.bindArray)


];
request_body.additionaldata(additionalData)





result = await client.security.cases.ediscoveryCases_by_id('ediscoveryCase-id').legalHolds.post(request_body = request_body)


```