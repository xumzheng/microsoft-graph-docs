---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DataSource();
requestBody.set@odatatype('microsoft.graph.security.siteSource');

additionalData = [
'site' => requestBody = Site();
		requestBody.setWebUrl('https://m365x809305.sharepoint.com/sites/Design-topsecret');


requestBody.setSite($site);

];
requestBody.setAdditionalData(additionalData);




result = await client.security().cases().ediscoveryCasesById('ediscoveryCase-id').searchesById('ediscoverySearch-id').additionalSources().post(requestBody);


```