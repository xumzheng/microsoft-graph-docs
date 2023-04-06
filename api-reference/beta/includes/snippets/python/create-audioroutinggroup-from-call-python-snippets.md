---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AudioRoutingGroup()
request_body.setId('oneToOne')

request_body.setRoutingMode(RoutingMode('onetoone'))

request_body.setSources(['632899f8-2ea1-4604-8413-27bd2892079f', ])

request_body.setReceivers(['550fae72-d251-43ec-868c-373732c2704f', ])



result = await client.communications.calls_by_id('call-id').audioRoutingGroups.post(request_body, headers=)


```