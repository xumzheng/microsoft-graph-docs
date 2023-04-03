---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = InboundFlow();
requestBody.set@odatatype('#microsoft.graph.industryData.inboundFlow');

requestBody.setDisplayName('My Inbound Flow');

requestBody.setEffectiveDateTime(DateTime('2022-03-12T16:40:46.924769+05:30'));

requestBody.setExpirationDateTime(DateTime('2023-03-12T16:40:46.924769+05:30'));



result = awaitclient.external().industryData().inboundFlowsById('inboundFlow-id').patch(requestBody);


```