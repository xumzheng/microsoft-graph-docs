---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Case();
requestBody.setDisplayName('My Case 1 - Renamed');

requestBody.setDescription('Updated description');

requestBody.setExternalId('Updated externalId');



result = await client.compliance().ediscovery().casesById('case-id').patch(requestBody);


```