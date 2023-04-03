---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = DataSource();
requestBody.set@odatatype('microsoft.graph.security.siteSource');

additionalData = [
'site' => requestBody = Site();
		requestBody.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite');


requestBody.setSite($site);

];
requestBody.setAdditionalData(additionalData);




requestResult = graphServiceClient.security().cases().ediscoveryCasesById('ediscoveryCase-id').searchesById('ediscoverySearch-id').additionalSources().post(requestBody);


```