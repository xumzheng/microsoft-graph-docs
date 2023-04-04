---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EdiscoveryHoldPolicy();
request_body.setDisplayname('My legalHold with sources');

request_body.setDescription('Created from Graph API');

additionalData = [
'userSources@odata.bind' => userSources@odatabind1 = ();
		userSources@odatabind1.set@odatatype('microsoft.graph.security.userSource');

		userSources@odatabind1.setEmail('SalesTeam@M365x809305.OnMicrosoft.com');


userSources@odata.bindArray []= userSources@odatabind1;
request_body.setUserSources@odatabind(userSources@odata.bindArray);


'siteSources@odata.bind' => siteSources@odatabind1 = ();
	siteSources@odatabind1.set@odatatype('microsoft.graph.security.siteSource');

siteSources@odatabind1Site = Site();
	siteSources@odatabind1Site.setWebUrl('https://m365x809305.sharepoint.com/sites/Design-topsecret');


siteSources@odatabind1.setSite($siteSources@odatabind1Site);

siteSources@odata.bindArray []= siteSources@odatabind1;
request_body.setSiteSources@odatabind(siteSources@odata.bindArray);


];
request_body.setAdditionalData(additionalData);




result = await client.security().cases().ediscoveryCasesById('ediscoveryCase-id').legalHolds().post(request_body);


```