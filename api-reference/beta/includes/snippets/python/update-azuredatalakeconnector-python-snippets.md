---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = IndustryDataConnector()
request_body.set@odatatype('microsoft.graph.industryData.azureDataLakeConnector')

request_body.setDisplayName('API Monitor 60201009')



result = await client.external_industryData_dataConnectorsby_id('industryDataConnector-id').patch(request_body)


```