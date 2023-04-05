---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InboundFlow()
request_body.set@odatatype('#microsoft.graph.industryData.inboundFlow')

request_body.setDisplayName('My Inbound Flow')

request_body.setEffectiveDateTime(DateTime('2022-03-12T16:40:46.924769+05:30'))

request_body.setExpirationDateTime(DateTime('2023-03-12T16:40:46.924769+05:30'))



result = await client.external_industryData_inboundFlowsby_id('inboundFlow-id').patch(request_body)


```