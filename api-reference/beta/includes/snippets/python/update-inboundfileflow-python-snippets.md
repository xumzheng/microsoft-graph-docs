---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new InboundFlow();
$requestBody.set@odatatype('#microsoft.graph.industryData.inboundFlow');

$requestBody.setDisplayName('My Inbound Flow');

$requestBody.setEffectiveDateTime(new DateTime('2022-03-12T16:40:46.924769+05:30'));

$requestBody.setExpirationDateTime(new DateTime('2023-03-12T16:40:46.924769+05:30'));



$requestResult = $graphServiceClient.external().industryData().inboundFlowsById('inboundFlow-id').patch($requestBody);


```