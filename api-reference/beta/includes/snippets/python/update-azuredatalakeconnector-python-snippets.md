---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IndustryDataConnector()
request_body.@odatatype = 'microsoft.graph.industryData.azureDataLakeConnector'

request_body.displayName = 'API Monitor 60201009'




result = await client.external.industryData.dataConnectors_by_id('industryDataConnector-id').patch(request_body = request_body)


```