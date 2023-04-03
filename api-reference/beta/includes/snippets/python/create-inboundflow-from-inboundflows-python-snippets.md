---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = InboundFlow();
requestBody.set@odatatype('#microsoft.graph.industryData.inboundFileFlow');

requestBody.setDataDomain(InboundDomain('educationrostering'));

requestBody.setDisplayName('Inbound rostering flow');

requestBody.setEffectiveDateTime(DateTime('2023-03-12T16:40:46.924769+05:30'));

requestBody.setExpirationDateTime(DateTime('2023-03-13T16:40:46.924769+05:30'));

additionalData = [
'dataConnector@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/dataConnectors/51dca0a0-85f6-4478-f526-08daddab2271', 
'year@odata.bind' => 'https://graph.microsoft.com/beta/external/industryData/years/ebf18762-ab92-487e-21d1-08daddab28bb', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.external().industryData().inboundFlows().post(requestBody);


```