---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InboundFlow()
request_body.@odatatype = '#microsoft.graph.industryData.inboundFlow'

request_body.displayName = 'My Inbound Flow'

request_body.effectiveDateTime = DateTime('2022-03-12T16:40:46.924769+05:30')

request_body.expirationDateTime = DateTime('2023-03-12T16:40:46.924769+05:30')



request_configuration = InboundFlowRequestBuilderPatchRequestConfiguration(
)


result = await client.external.industryData.inboundFlows_by_id('inboundFlow-id').patch(request_body = request_body)


```