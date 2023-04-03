---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = IndustryDataConnector();
requestBody.set@odatatype('microsoft.graph.industryData.azureDataLakeConnector');

requestBody.setDisplayName('API Monitor 60201009');



requestResult = graphServiceClient.external().industryData().dataConnectorsById('industryDataConnector-id').patch(requestBody);


```