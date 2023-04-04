---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Simulation()
request_body.setId('2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc')

request_body.setStatus(SimulationStatus('cancelled'))

additionalData = [
'@odata.etag' => '\"0100aa9b-0000-0100-0000-6396fa270000\"', 
];
request_body.setAdditionalData(additionalData)




result = await client.security.attackSimulation.simulationsById('simulation-id').patch(request_body)


```