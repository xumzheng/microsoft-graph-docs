---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InboundFlow()
request_body.set@odatatype('#microsoft.graph.industryData.inboundFileFlow')

request_body.setDisplayName('Updated flow name')



result = await client.external.industryData.inboundFlows_by_id('inboundFlow-id').patch(request_body)


```