---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = IndustryDataConnector();
requestBody.set@odatatype('microsoft.graph.industryData.azureDataLakeConnector');

requestBody.setDisplayName('API Monitor 60201009');



result = await client.external().industryData().dataConnectorsById('industryDataConnector-id').patch(requestBody);


```