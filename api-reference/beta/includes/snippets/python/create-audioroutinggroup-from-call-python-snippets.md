---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = AudioRoutingGroup();
requestBody.setId('oneToOne');

requestBody.setRoutingMode(RoutingMode('onetoone'));

requestBody.setSources(['632899f8-2ea1-4604-8413-27bd2892079f', ]);

requestBody.setReceivers(['550fae72-d251-43ec-868c-373732c2704f', ]);



result = await client.communications().callsById('call-id').audioRoutingGroups().post(requestBody);


```