---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = Simulation();
requestBody.setId('2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc');

requestBody.setStatus(SimulationStatus('cancelled'));

additionalData = [
'@odata.etag' => '\"0100aa9b-0000-0100-0000-6396fa270000\"', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.security().attackSimulation().simulationsById('simulation-id').patch(requestBody);


```