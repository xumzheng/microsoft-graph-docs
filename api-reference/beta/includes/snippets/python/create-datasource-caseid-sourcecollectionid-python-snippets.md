---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = DataSource();
requestBody.set@odatatype('microsoft.graph.ediscovery.userSource');

additionalData = [
'email' => 'badguy@contoso.com', 
];
requestBody.setAdditionalData(additionalData);




result = await client.compliance().ediscovery().casesById('case-id').sourceCollectionsById('sourceCollection-id').additionalSources().post(requestBody);


```