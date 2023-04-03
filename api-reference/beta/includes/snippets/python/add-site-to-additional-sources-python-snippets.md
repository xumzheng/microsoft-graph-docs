---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DataSource();
requestBody.set@odatatype('microsoft.graph.ediscovery.siteSource');

additionalData = [
'site' => requestBody = Site();
		requestBody.setWebUrl('https://contoso.sharepoint.com/sites/SecretSite');


requestBody.setSite($site);

];
requestBody.setAdditionalData(additionalData);




result = await client.compliance().ediscovery().casesById('case-id').sourceCollectionsById('sourceCollection-id').additionalSources().post(requestBody);


```