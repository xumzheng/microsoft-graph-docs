---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InboundFlow()
request_body.@odatatype = '#microsoft.graph.industryData.inboundFileFlow'

request_body.displayName = 'Updated flow name'




result = await client.external.industryData.inboundFlows_by_id('inboundFlow-id').patch(request_body = request_body)


```